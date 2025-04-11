# Necessity and Sufficiency Analysis for Hate Speech Detection

This repository contains the implementation of our project on **interpreting hate speech classifiers** using **necessity and sufficiency metrics**, inspired by the method proposed in *Balkir et al. (2022)*.

Our work focuses on reimplementing this framework using **DistilBERT** and **RoBERTa** classifiers trained on real and synthetic hate speech datasets, and analyzing their behavior towards the identity target **"black people"**.

---

## 🔍 Repository Structure

| File / Folder | Description |
|---------------|-------------|
| `Notebook_Base_1.ipynb` | **Main Kaggle notebook** created by the first collaborator. It contains dataset loading, ILM (GPT-2) training, perturbation generation, and necessity/sufficiency computation. |
| `NLP_classif.ipynb` | Notebook used in **Google Colab** to train both DistilBERT and RoBERTa classifiers. Created by the first collaborator. |
| `analysis_of_results_Roberta.ipynb` | Analysis notebook focused on **RoBERTa-based classifiers** (necessity/sufficiency + SHAP/LIME), authored by the first collaborator. |
| `Notebook2.ipynb` | Adapted from `Notebook_Base_1.ipynb` by the second collaborator. Focuses on **DistilBERT-based analysis** and further extensions. |
| `perturbation_functions.py` | Contains core functions for generating perturbations, masking tokens, and infilling using the ILM. |
| `train.py` | Helper script for training classifiers. |
| `Weights/` | Folder containing pretrained model checkpoints. |
| `ilm/` | Code for In-filling Language Model. |
| `hatecheck-data/` | Contains the HateCheck test suite used to evaluate model fairness and consistency. |
| `Data/`, `test_trainer/logs/`, `__pycache__/` | Supporting assets, logs, and runtime files. |

---

## ⚠️ Notebook Preview Issues

The following notebooks were created and executed in **Google Colab**, and may not render properly on GitHub due to widget metadata issues. You can:

- ✅ **Download** them and open locally in Jupyter.
- ✅ **View them directly in Colab** via the links below:

- [🔗 Classifier Training Notebook (NLP_classif.ipynb)](https://colab.research.google.com/drive/1TEqwfQjRNcbPXnYx6dYxZ6b1X8aBiyO8?usp=sharing)
- [🔗 DistilBERT Analysis Notebook (Notebook2.ipynb)](https://drive.google.com/file/d/11xLKLoixoJg5Z77ctgKd7wlVVt1pC75-/view?usp=sharing)

