# Perspective-Aware Natural Language Inference (PANLI) Dataset

> A benchmark dataset for studying natural language inference (NLI) with diverse human perspectives, based on real-world vaccination discourse.

The PANLI dataset is a natural language inference (NLI) benchmark consisting of premise-hypothesis pairs constructed from naturally occurring and independently authored texts extracted from the Vaccination Corpus. These pairs underwent only minimal automated post-processing, preserving their authenticity and reflecting real-world language use.

A key feature of the PANLI dataset is its perspective-aware design. Each premise-hypothesis pair receives at least one judgment from the author of the premise, and possibly one or more additional judgments from sources mentioned in the premise. These relative relationships between premises and hypotheses are referred to as *perspective units*.

The dataset is described in the following thesis:

> van Son, C. M. (2024). *Representative Resources for Perspective-Aware Natural Language Inference* (PhD thesis, Vrije Universiteit Amsterdam). [https://doi.org/10.5463/thesis.644](https://doi.org/10.5463/thesis.644)

## Related Projects
- [panli-crowdtruth](https://github.com/cltl/panli-crowdtruth) — Analysis of the PANLI dataset using the CrowdTruth framework.
- [panli-models](https://github.com/cltl/panli-models) — Evaluation of Transformer models on PANLI.
- [vaccination-corpus](https://github.com/cltl/vaccination-corpus) -  Source corpus for premise-hypothesis pair extraction.

## Repository Contents

```bash
📁 data/
  ├── prolific_results.csv         # Raw individual annotations (via Prolific)
  └── panli.csv                    # Aggregated results + CrowdTruth metrics

📁 notebooks/
  └── explore_panli.ipynb          # Jupyter notebook for dataset exploration
```



## Explore the data

You can explore the dataset via Jupyter notebooks. Use [Poetry](https://python-poetry.org/) to manage dependencies.

1. **Install Poetry** (if needed)

    ```bash
    curl -sSL https://install.python-poetry.org | python3 -
    ```
    Or see the [official Poetry installation guide](https://python-poetry.org/docs/#installation).

2. **Install project dependencies**

    ```bash
    poetry install
    ```

3. **Launch Jupyter Notebook**

    ```bash
    poetry run jupyter notebook
    ```


## Citation

If you use this dataset in your research, please cite:

* van Son, C. M. (2024). *Representative Resources for Perspective-Aware Natural Language Inference* (PhD thesis, Vrije Universiteit Amsterdam). [https://doi.org/10.5463/thesis.644](https://doi.org/10.5463/thesis.644)

    <details>
    <summary>BibTeX</summary>
    ```bibtex
    @phdthesis{ba18bc83a2be4b29805c6b91aaa9a152,
        title = "Representative Resources for Perspective-Aware Natural Language Inference",
        author = "{van Son}, {Chantal Michelle}",
        year = "2024",
        month = nov,
        day = "1",
        doi = "10.5463/thesis.644",
        language = "English",
        type = "PhD-Thesis - Research and graduation internal",
        school = "Vrije Universiteit Amsterdam",
    }
    ```
    </details>

