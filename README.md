
#  CS772 Project: AutoElicit-Augmented Active Learning

##  Group Members
- **Member 1**: Chaitanya Bramhapurikar (230305)
- **Member 2**: Naveen Kumar (220699)
- **Member 3**: Riyanshi (220903)
- **Member 4**: Shubhanshu Mishra (221048)
---

##  Project Overview

### IDEA 1:
In this project, we explored the integration of **AutoElicit**, a large language model (LLM)-based prior elicitation method, into **active learning** for **natural language processing (NLP)**—specifically for binary sentiment classification using the SST-2 dataset.

We conducted **six experiments** in total:
- **2 experiments** using LLM-based augmentation via AutoElicit.
- **4 experiments** without LLM assistance (standard active learning using uncertainty sampling, random sampling, and query-by-committee strategies).

Our goal was to evaluate whether LLMs can enhance sample efficiency by synthetically generating informative samples during active learning phases.

---

##  Directory Structure

```
CS-772-Project/
├── Idea1/
│   ├── with-autoelicit/
│   │   ├── naive_active_learning_with_autoelicit.ipynb     
│   │   └── autoelicit_with_uncertainity_sampling.ipynb     
│   └── naive-active-learning/
│       ├── without_active_learning_at_all.ipynb                         # Baseline model
│       ├── naive_active_leaarning_without_any_modifications.ipynb      # Random sampling
│       ├── active_learning_with_query_by_committe.ipynb                # [Colab](https://colab.research.google.com/drive/1WabVQjhW4oWjyHidX5cl9Wlx_GIgkJxY?usp=sharing)
│       └── active_learning_with_uncertainity_sampling.ipynb            # [Colab](https://colab.research.google.com/drive/1DJt2v53FR86u2GNGA08Kj5YfqFQLBTK4?usp=sharing)
├── Seed-papers/
│   ├── autoelicit-using-large-language-models-for-expert-prior-elicitation-in-predictive-modeling.pdf
│   ├── understanding-uncertainity-sampling.pdf
│   ├── model-agnostic-meta-learning-for-fast-adaptation-of-deep-networks.pdf
│   └── query-by-committe.pdf
├── project_proposal.pdf
└── README.md
```

### `with-autoelicit/`
This folder contains experiments that incorporate AutoElicit to augment the active learning process:
- `naive_active_learning_with_autoelicit.ipynb`: Active learning with AutoElicit-augmented samples.
- `autoelicit_with_uncertainity_sampling.ipynb`: Active learning using AutoElicit for generating informative samples combined with uncertainty sampling.

### `naive-active-learning/`
This folder contains experiments that use traditional active learning techniques without the augmentation of AutoElicit:
- `without_active_learning_at_all.ipynb`: A baseline model with no active learning.
- `naive_active_leaarning_without_any_modifications.ipynb`: Traditional random sampling-based active learning.
- `active_learning_with_query_by_committe.ipynb`: Active learning using query-by-committee strategy. [Colab Link](https://colab.research.google.com/drive/1WabVQjhW4oWjyHidX5cl9Wlx_GIgkJxY?usp=sharing)
- `active_learning_with_uncertainity_sampling.ipynb`: Active learning with uncertainty sampling. [Colab Link](https://colab.research.google.com/drive/1DJt2v53FR86u2GNGA08Kj5YfqFQLBTK4?usp=sharing)

---


## ⚙️ How to Run

Some experiments can be executed directly as Jupyter notebooks, while others are hosted on Google Colab (links included above).

You may need to install the following libraries:
```bash
pip install transformers datasets scikit-learn
```

---

##  Notes

- **Dataset Used**: SST-2 (Stanford Sentiment Treebank) via HuggingFace Datasets
- **LLM**: AutoElicit-based augmentation with Ollama 
- **Query Strategies**: Random, Uncertainty Sampling, Query by Committee

---
