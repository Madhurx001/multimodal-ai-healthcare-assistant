# System Architecture

## Current Design
The proposed system has five major stages:

1. **Data Acquisition**
   - Medical images
   - Structured clinical information

2. **Preprocessing**
   - Image resizing, normalization and augmentation
   - Missing-value handling, encoding and scaling for clinical data

3. **Modality-Specific Feature Extraction**
   - CNN/deep-learning model for medical images
   - Machine-learning or neural model for structured data

4. **Multimodal Fusion**
   - Image and clinical feature representations are combined before prediction

5. **Explainability**
   - Grad-CAM: highlights influential image regions
   - SHAP: estimates contribution of clinical features
   - Natural-language layer: presents the result in an understandable form

## Validation So Far
The architecture has been validated at the design level through:
- A literature survey of 20 research papers
- Comparison with the xHAIM base paper
- Feasibility analysis for an undergraduate implementation

No end-to-end experimental validation has been completed yet.
