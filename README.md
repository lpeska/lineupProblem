# The Lineup Problem: An Opportunity for Late Interaction in Candidate Retrieval
This repository contains the companion Jupyter notebook for the manuscript submitted to RecSys 2026 Research & Practice Notes track:

> **The Lineup Problem: An Opportunity for Late Interaction in Candidate Retrieval**

The notebook reproduces the complete experimental pipeline presented in the paper, including:

- construction of the NBA game catalog from the ESPN 2025–26 schedule,
- indexing the same collection using **BM25**, **single-vector dense retrieval (Qwen3)**, and **late interaction (ColBERT)**,
- generation of three user profiles:
  - player preference,
  - geographic preference,
  - compound preference,
- evaluation using **MRR** and **Recall@R**,
- visualization of the reported results and illustrative retrieval examples.

The notebook is intentionally self-contained and organized as a step-by-step walkthrough of the experiments described in the paper. The NBA games dataset is reconstructed automatically as part of the notebook. We plan to publish the resulting dataset on Hugging Face after the review process is complete; until then, we refrain from releasing it to preserve the anonymity of the submission.

## Requirements

The notebook depends on:

- Python 3.11+
- `numpy`
- `matplotlib`
- `sentence-transformers`
- `pylate`
- `topk-sdk`

Additionally, you will need a TopK account and a valid **TopK API key**. These can be configured either through the notebook or via the `TOPK_API_KEY` environment variable. See the TopK documentation [https://docs.topk.io/introduction] for details.

## Running the Notebook

1. Install the required Python packages.
2. Configure the TopK endpoint and API credentials.
3. Execute the notebook from top to bottom.

All indices are built directly from the notebook, after which the evaluation and visualizations can be reproduced automatically.

## Repository Structure

```
the-lineup-problem.ipynb    # Complete reproducibility notebook
README.md                   # This file
```

## Citation

TODO
