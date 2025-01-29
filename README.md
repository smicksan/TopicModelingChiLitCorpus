
# Topic Modeling with LDA on the ChiLit Corpus

**Author:** Sandra Mickwitz  
**Institution:** Università Cattolica del Sacro Cuore    

<p align="center">
   <img src="https://github.com/mahlberg-lab/corpora/blob/master/images/ChiLit_0.4.jpg" width="800">
</p>

## Introduction

The aim of this project is to train a **Latent Dirichlet Allocation (LDA)** model to analyze and understand the **topics** in the **ChiLit Corpus** from [mahlberg-lab/corpora](https://github.com/mahlberg-lab/corpora/tree/a020b2a7153baf8849056be833861ecb3d77e7a1/ChiLit).

A key research question during model training was:  
**What is the ideal number of topics?**  
The goal was to find a balance between **not too many fine-grained topics** and **not too few overly broad topics**.

## ChiLit Corpus Description

The **ChiLit Corpus** is used in this notebook.  
The corpus can be accessed [here](https://github.com/mahlberg-lab/corpora/tree/a020b2a7153baf8849056be833861ecb3d77e7a1/ChiLit).

Additionally, a **notebook** is available for **preprocessing** the corpus.

## Corpus Statistics

| **Metric**                 | **Unprocessed Files** | **Processed Files** | **Why the Change?**                                   |
|---------------------------|-----------------------|---------------------|------------------------------------------------------|
| **Total Words (Tokens)**   | 5,404,761             | 2,191,892           | Stopwords & punctuation removed                      |
| **Unique Words (Tokens)**  | 70,728                | 51,673              | Slight reduction, but more meaningful words remain   |
| **Lexical Richness**       | 0.0131                | 0.0236              | Fewer redundant words, unique word ratio increased   |

## Topic Modeling with OCTIS

This project utilizes [OCTIS (Optimized Configuration of Topic Models)](https://github.com/MIND-Lab/OCTIS/blob/master/README.rst?plain=1), a **Python library** designed to facilitate **topic model training and evaluation**.

### OCTIS provides:
- **Preprocessing tools** to clean and prepare text data.
- **Multiple topic modeling algorithms**, including:
  - **LDA (Latent Dirichlet Allocation)**
  - **ProdLDA (Product of Experts LDA)**
  - **ETM (Embedded Topic Model)**
- **Evaluation metrics** such as:
  - **Topic Diversity**
  - **Topic Coherence**
- **Hyperparameter optimization** for tuning the number of topics.

For more details, visit the [official repository](https://github.com/MIND-Lab/OCTIS/blob/master/README.rst).

## OCTIS Citation

[Click to read the paper](https://www.aclweb.org/anthology/2021.eacl-demos.31)!

```bibtex
@inproceedings{terragni2020octis,
    title={{OCTIS}: Comparing and Optimizing Topic Models is Simple!},
    author={Terragni, Silvia and Fersini, Elisabetta and Galuzzi, Bruno Giovanni and Tropeano, Pietro and Candelieri, Antonio},
    year={2021},
    booktitle={Proceedings of the 16th Conference of the European Chapter of the Association for Computational Linguistics: System Demonstrations},
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/2021.eacl-demos.31",
    pages = "263--270",
}
```

## Short Information About the Complete ChiLit Corpus

The **GLARE 19th Century Children’s Literature Corpus** is part of **CLiC!**  
📌 Blog post: [ChiLit: the GLARE 19th Century Children’s Literature Corpus in CLiC](https://blog.bham.ac.uk/glareproject/2018/02/14/chilit-the-glare-19th-century-childrens-literature-corpus-in-clic/)

### Corpus Overview
- Developed as part of the **MC-Project GLARE** (*Exploring Gender in Children’s Literature from a Cognitive Corpus Stylistic Perspective*).
- Directed by **Anna Čermáková** and **M. Mahlberg**.
- **71 books** (*35 by female, 36 by male authors*).
- **38 authors** (*14 female, 24 male*).
- Published between **1826-1911**.
- **4,480,386 words** in total.
- **Source:** [Gutenberg Project](https://www.gutenberg.org/) (Public Domain).

## Reference

Čermáková, A. (2018, 14 February).  
[ChiLit: the GLARE 19th Century Children’s Literature Corpus in CLiC](https://blog.bham.ac.uk/glareproject/2018/02/14/chilit-the-glare-19th-century-childrens-literature-corpus-in-clic/)  
Retrieved from *University of Birmingham Blog*.

📢 **Feedback and contributions are welcome!**  
Feel free to submit issues or pull requests.
