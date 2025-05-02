CS772 Project: AutoElicit-Augmented Active Learning for NLP
Group Members
Member 1: Chaitanya Bramhapurikar (230305)
Member 2: Naveen Kumar (220699)
Member 3: Riyanshi (220903)
Member 4: Shubhanshu Mishra (221048)

Project Overview
IDEA1 : In this project we explored the integration of AutoElicit, a large language model (LLM)-based prior elicitation method, into active learning for natural language processing (NLP)—specifically binary sentiment classification using the SST-2 dataset.
We conduct six experiments in total:

2 experiments using LLM-based augmentation via AutoElicit.

4 experiments without LLM assistance (standard active learning using uncertainty sampling or random strategies).

Our aim is to evaluate whether LLMs can enhance sample efficiency by synthetically generating informative samples during active learning phases.

Directory Structure
bash
Copy
Edit
CS-772-Project/
├── Idea1/
│   ├── with-autoelicit/
│   │   ├── naive_active_learning_with_autoelicit.ipynb     
│   │   └── autoelicit_with_uncertainity_sampling.ipynb     
│   └── naive-active-learning/
│       ├── without_active_learning_at_all.ipynb       # baseline model
│       ├── naive_active_leaarning_without_any_modifications.ipynb       # Active learning with random sampling
│       ├── active_learning_with_query_by_committe.ipynb  # [[Google Colab Link](https://colab.research.google.com/drive/1WabVQjhW4oWjyHidX5cl9Wlx_GIgkJxY?usp=sharing)]
│       └── active_learning_with_uncertainity_sampling.ipynb    # [[Google Colab Link](https://colab.research.google.com/drive/1DJt2v53FR86u2GNGA08Kj5YfqFQLBTK4?usp=sharing)]
├── Seed-papers/
│   ├── autoelicit-using-large-language-models-for-expert-prior-elicitation-in-predictive-modeling.pdf
│   ├── understanding-uncertainity-sampling.pdf
│   ├── model-agnostic-meta-learning-for-fast-adaptation-of-deep-networks.pdf
│   └── query-by-committe.pdf
├── project_proposal.pdf
├── README.md

