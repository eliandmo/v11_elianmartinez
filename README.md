# BERTopic Thesis Notebook

This repository contains the materials used to reproduce and review the
BERTopic-based analysis developed for the thesis project on narrative structures
in scientific publications related to news media.

## Google Colab Notebook

The main notebook can be accessed directly through Google Colab:

[Open notebook in Google Colab](https://colab.research.google.com/drive/1nBhS0jCXixKShqDUBELZF9kBDaEQMYs0?usp=sharing)

This notebook includes the complete workflow used for the analysis:

- loading the Scopus corpus,
- abstract-based BERTopic modeling,
- embedding and hyperparameter comparison,
- model diagnostics,
- OpenAI-assisted topic labeling,
- topic figures and tables,
- outlier review.

## Optional Llama 3.1 Notebook

An alternative notebook using Llama 3.1 is also included as an optional
API-free labeling workflow:

```text
notebooks/bertopic_thesis_reanalysis_llama31_local_optional.ipynb
```

This version is intended for users who do not have access to an OpenAI API key.
Its labels may differ from the OpenAI-assisted labels because local LLM outputs
depend on the selected model, runtime configuration, quantization, and available
GPU resources.

## Data Used

The analysis uses the following files:

```text
data/scopus_final_with_references.csv
data/thesaurus_bibliometrix_elian.csv
```

The first file contains the final Scopus corpus used for the bibliometric and
BERTopic analyses. The second file contains the thesaurus used for term
normalization.

## Selected PDF Outputs



These figures summarize the model comparison, topic prevalence, representative
c-TF-IDF terms, and the UMAP projection of BERTopic topics.

## Note

The OpenAI-assisted labeling step requires a private API key. The key is not
included in this repository.
