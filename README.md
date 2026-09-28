# Evaluation of Data Augmentation Techniques for Code-Switched Speech Recognition Systems

This repository contains the implementation and experimental results for an Honours research project investigating the effect of data augmentation techniques on Automatic Speech Recognition (ASR) for **Sepedi–English code-switched speech**.

## Research Overview

The study evaluates whether data augmentation can improve the performance and generalisation of a Whisper-based ASR system in a low-resource, code-switched speech setting.

The experiments use the **SPCS (Sepedi Speech Corpus)** and fine-tune **OpenAI Whisper-Tiny** using different augmentation strategies.

## Data Augmentation Techniques

The following configurations were evaluated:

* **Baseline** – No data augmentation
* **Noise Injection** – Addition of controlled background noise
* **Speed Perturbation** – Modification of speech speed
* **Pitch Shifting** – Modification of speech pitch
* **SpecAugment** – Time and frequency masking

## Evaluation Metrics

Model performance was evaluated using:

* **Word Error Rate (WER)**
* **Character Error Rate (CER)**
* **Validation/Test Loss**

The experiments compare each augmentation technique against a non-augmented baseline.

## Repository Structure

```text
SPCS/
├── Code/
│   ├── SPSC.ipynb
│   ├── Untitled.ipynb
│   ├── Untitled1.ipynb
│   ├── Untitled2.ipynb
│   └── Untitled3.ipynb
│
├── graph_results/
│   ├── baseline_whisper/
│   ├── noise_whisper/
│   ├── pitch_whisper/
│   ├── specaugment_whisper/
│   ├── speed_whisper/
│   ├── test/
│   └── _comparison/
│
├── manifests/
│   ├── train.csv
│   ├── valid.csv
│   └── test.csv
│
├── data/          # Not included in repository
├── models/        # Not included in repository
└── models_result/ # Not included in repository
```

## Dataset

The experiments use the **SPCS Speech Corpus**. The original audio dataset is not included in this repository due to dataset size and distribution restrictions.

The repository contains the generated dataset manifests used for training, validation, and testing.

## Model

The experiments use:

**OpenAI Whisper-Tiny**

Whisper is a multilingual speech recognition model developed by OpenAI and trained on a large-scale collection of multilingual and multitask supervised data.

## Technologies

* Python
* PyTorch
* Hugging Face Transformers
* OpenAI Whisper
* Librosa
* Pandas
* NumPy
* Jupyter Notebook
* Matplotlib

## Research Focus

The project focuses on:

* Low-resource speech recognition
* Sepedi–English code-switching
* Automatic Speech Recognition
* Data augmentation
* Whisper fine-tuning
* Model evaluation and generalisation

## Author

**Lindokuhle Zulu**
University of Limpopo
Honours in Computer Science

## Research Project

**Title:** Evaluation of Data Augmentation Techniques for Code-Switched Speech Recognition Systems

This repository contains code, experiment configurations, evaluation results, and visualisations associated with the research project.
