# Subword Evenness and Cross-Lingual Transfer in Multilingual Language Models

This repository documents my contribution to the paper:

**"Subword Evenness (SuE) as a Predictor of Cross-lingual Transfer to Low-resource Languages"**  
by Olga Pelloni, Anastassia Shaitarova, and Tanja Samardzic  
[https://aclanthology.org/2022.emnlp-main.503/](https://aclanthology.org/2022.emnlp-main.503/)

🔗 Full codebase: [olgapelloni/subword_evenness](https://github.com/olgapelloni/subword_evenness)

---

## Overview

Pre-trained multilingual models like **mBERT**, **XLM-R**, and **mT5** are widely used to improve performance on NLP tasks in **low-resource languages** via **cross-lingual transfer**. Traditionally, English is chosen as the transfer language, but recent evidence shows this may not be optimal.

This project introduces **Subword Evenness (SuE)** — a novel metric that predicts the effectiveness of a source language in cross-lingual transfer. We demonstrate that **non-Latin, non-alphabetic scripts** (e.g., Asian languages) tend to yield better results in **Masked Language Modeling (MLM)** tasks for a diverse set of 30 low-resource languages.

---

## My Contribution

As second author and contributor, I was responsible for:

- Preparing multilingual Hugging Face `Dataset` objects from raw text for over 30 low- and high-resource languages, including genre balancing, token curation, and metadata management  
- Designing and running training pipelines for **mBERT** and **mT5** using Hugging Face scripts, including checkpointing, perplexity evaluation, and correlation analysis across language pairs  
- Setting up and maintaining experiment infrastructure across multiple servers, optimizing training parameters, and automating evaluation workflows  
- Co-authoring the paper and supporting documentation

---

## Citation

If you use the paper or its associated code, please cite:
@inproceedings{pelloni-etal-2022-subword,
title = "Subword Evenness (SuE) as a Predictor of Cross-lingual Transfer to Low-resource Languages",
author = "Pelloni, Olga and Shaitarova, Anastassia and Samardzic, Tanja",
booktitle = "Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing",
year = "2022",
url = "https://aclanthology.org/2022.emnlp-main.503"
}
