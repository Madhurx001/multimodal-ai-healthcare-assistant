# Multimodal AI-Based Healthcare Assistant with Explainable AI

## Project Overview
This major project explores a multimodal AI-based healthcare decision-support system that combines medical images with structured clinical information and provides interpretable predictions.

The proposed system focuses on three forms of explanation:

- **Grad-CAM** for visual explanation of medical-image predictions
- **SHAP** for feature-level explanation of structured clinical data
- **Natural-language explanations** for presenting results in an understandable form

> **Important:** This project is intended as an academic decision-support prototype and is not designed to replace healthcare professionals or provide autonomous diagnosis or prescriptions.

## Current Project Status
The project is currently in the **design and initial implementation-planning stage**.

Completed so far:
- Literature survey of **20 recent research papers**
- Selection of **xHAIM** as the base paper
- Identification of the research gap
- Definition of project objectives and scope
- Proposed multimodal system architecture
- Selection of planned XAI techniques: Grad-CAM and SHAP
- Phase-I report and presentation

Not yet completed:
- Final dataset selection
- Full model training
- End-to-end prototype
- Experimental evaluation
- UI integration

## Base Paper
**Holistic AI in Medicine; Improved Performance and Explainability (xHAIM)**

The base paper combines multimodal patient information with grounded clinical explanations. Our proposed work studies a smaller and more feasible academic architecture with stronger **modality-specific explainability**.

## Research Gap
The literature survey identified scope for combining:

1. **Visual explanation** for medical images
2. **Feature-level explanation** for structured clinical data
3. **Human-readable natural-language explanation**

within a single lightweight multimodal framework.

The selected base paper also highlights challenges related to computational overhead, dependence on medical knowledge sources, and broader external validation.

## Proposed Architecture
```text
Medical Image ──> Image Preprocessing ──> CNN ────────┐
                                                     │
                                                     ├──> Multimodal Fusion ──> Prediction
                                                     │                         │
Clinical Data ──> Data Preprocessing ──> ML Model ───┘                         │
                                                                               ├──> Grad-CAM
                                                                               ├──> SHAP
                                                                               └──> Natural-Language Explanation
```

## Repository Structure
```text
.
├── README.md
├── requirements.txt
├── .gitignore
├── data/
│   └── README.md
├── docs/
│   ├── architecture.md
│   ├── literature-survey.md
│   └── midterm-status.md
├── notebooks/
│   └── README.md
├── results/
│   └── README.md
├── screenshots/
└── src/
    └── README.md
```

## Planned Technology Stack
- Python
- TensorFlow / PyTorch
- Scikit-learn
- OpenCV
- SHAP
- Grad-CAM
- Pandas / NumPy
- Matplotlib

## Next Steps
1. Finalize the clinical prediction task and public multimodal dataset
2. Build the image preprocessing pipeline
3. Build the structured clinical-data pipeline
4. Train unimodal baseline models
5. Implement multimodal fusion
6. Integrate Grad-CAM and SHAP
7. Add natural-language explanation layer
8. Evaluate performance and explainability
9. Build a simple user-facing prototype

## Academic Status
This repository documents the ongoing B.Tech Major Project work and will be updated as implementation and experimental results become available.
