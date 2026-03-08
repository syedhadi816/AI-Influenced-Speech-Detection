# AI-Influenced Speech Detection

[![DOI](https://img.shields.io/badge/DOI-10.26153%2Ftsw%2F61304-0077b6?style=flat-square)](https://doi.org/10.26153/tsw/61304)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.x-3776ab?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat-square&logo=jupyter&logoColor=white)](https://jupyter.org/)

An interpretable, feature-based framework for detecting **plagiarized or AI-influenced speech** in spoken language assessments. This repository accompanies the research presented at the **National Council for Measurement in Education (NCME)** annual meeting (Denver, CO, 2025) and the associated publication.

---

## 📄 Publication

**Automated Plagiarism Detection in Spoken Responses using Linguistic and Acoustic Features**

- **Authors:** Syed Abdul Hadi  
- **DOI:** [10.26153/tsw/61304](https://doi.org/10.26153/tsw/61304)  
- **Institutional repository:** [UT Austin Texas ScholarWorks](https://doi.org/10.26153/tsw/61304)  
- **Keywords:** AI, Education, Test Security, Language Assessment  

If you use this work in your research, please cite the paper (see [CITATION](#citation) below).

---

## 🎯 Overview

The proliferation of generative AI tools has raised concerns about the **authenticity of responses** in spoken language assessments. This project presents a machine learning framework that detects AI-influenced or plagiarized speech by analyzing **speech delivery** in addition to content—going beyond traditional content-only plagiarism detection.

### Key contributions

- **Linguistic and acoustic feature set:** Speech rate, pause patterns, lexical richness, prosody, and energy entropy to distinguish spontaneous vs. nonspontaneous responses.  
- **Interpretable models:** Ten classifiers (SVM, MLP, EBM, etc.) with emphasis on explainability.  
- **Strong performance:** SVM and MLP achieve **89% accuracy** on 640 audio samples from a high-stakes English language proficiency test, outperforming content-based baselines.  
- **Statistical validation:** Feature discriminability validated via tests on both mean and variance across spontaneous and AI-influenced speech.

---

## 📁 Repository structure

```
AI-Influenced-Speech-Detection/
├── README.md
├── LICENSE
├── CITATION.cff
├── requirements.txt
├── .gitignore
└── AI_Influenced_Speech_Detection_and_Analysis.ipynb   # Main analysis notebook
```

---

## 🚀 Getting started

### Requirements

- **Python 3.x**  
- **Jupyter** (for running the notebook)  
- Dependencies used in the notebook (e.g., `numpy`, `pandas`, `scikit-learn`, and audio/linguistic libraries as defined in the notebook)

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/syedhadi816/AI-Influenced-Speech-Detection.git
   cd AI-Influenced-Speech-Detection
   ```

2. **Create a virtual environment (recommended)**
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   The notebook may use additional libraries (e.g. for audio); install any missing packages as prompted.

4. **Run the notebook**
   ```bash
   jupyter notebook AI_Influenced_Speech_Detection_and_Analysis.ipynb
   ```

### Data

The analysis in the paper uses **640 audio samples** from a high-stakes English language proficiency assessment. Due to test security and data privacy, the dataset is not included in this repository. The notebook documents the feature extraction and modeling pipeline so it can be adapted to compatible audio datasets.

---

## 📊 Methods (summary)

| Component        | Description |
|-----------------|-------------|
| **Features**    | Linguistic (e.g., lexical richness, fluency) and acoustic (speech rate, pauses, prosody, energy entropy). |
| **Models**      | SVM, MLP, EBM, and seven other classifiers; SVM and MLP reported at 89% accuracy. |
| **Interpretability** | Feature-based design and use of explainable models (e.g., EBM) for transparency. |

---

## 📜 Citation

If you use this code or the associated paper in your work, please cite:

```bibtex
@article{hadi2025ai,
  author    = {Hadi, Syed Abdul},
  title     = {AI-Influenced Speech Detection in Educational Assessments Using Linguistic and Acoustic Features},
  year      = {2025},
  publisher = {Texas ScholarWorks},
  doi       = {10.26153/tsw/61304},
  url       = {https://doi.org/10.26153/tsw/61304}
}
```

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Syed Abdul Hadi**  
- GitHub: [@syedhadi816](https://github.com/syedhadi816)  
- Research: Office of Institutional Research and Analysis (OIRA), The University of Texas at Austin  

---

*This work supports test security and fairness in spoken language assessments by enabling more reliable detection of AI-influenced or non-spontaneous responses.*
