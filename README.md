# Squishy Robotics - Wildfire Multimodal Forecasting

This repository hosts the code, datasets, and documentation for a research project conducted under the **Berkeley Expert Systems Technologies (BEST) Lab** in collaboration with **Squishy Robotics**, UC Berkeley.  
The project develops a **descriptor-guided multimodal forecasting framework** for wildfire spread and intensity prediction, integrating RGB, IR, and textual descriptors into an interpretable deep-learning pipeline for real-time robotic deployment.

---

## Overview

The research was conducted as part of the **Wildfire Response Team** within the BEST Lab from **January 2025 – May 2025**.  
The goal was to enhance the accuracy and interpretability of wildfire prediction models by integrating **multi-sensor visual data** with **textual event descriptors**, improving decision support for autonomous field robots deployed in disaster-response operations.  
This framework forms part of Squishy Robotics’ ongoing efforts to create adaptive, AI-powered situational awareness tools for emergency environments.

---

## Methodology

### Data Preparation

- Conducted **exploratory data analysis (EDA)** on the **Corsican Fire Database (CFDB)** to assess data sparsity, modality imbalance, and annotation gaps.  
- Implemented **computer-vision and Gemini-based augmentation pipelines** for RGB and IR imagery, enhancing coverage and improving descriptor completeness.  
- Normalized and synchronized multimodal data streams, aligning spatial, temporal, and descriptive metadata for downstream model training.

### Model Architecture

- Designed a **descriptor-guided multimodal forecasting framework** combining:  
  - **RGB and IR encoders** using **EfficientNet** and **Vision Transformer (ViT)** backbones for spatial-temporal feature extraction.  
  - **Textual descriptor embeddings** generated from **BERT** for contextual awareness of fire conditions and metadata.  
  - **LSTM-based late fusion** to capture temporal dynamics across visual and textual streams.  
- Trained and evaluated models on CFDB subsets for **fire-spread trajectory** and **intensity distribution** forecasting.

### Validation and Integration

- Assessed model performance across multimodal fusion strategies, emphasizing prediction stability and interpretability.  
- Deployed the trained forecasting module within **Squishy Robotics’ autonomous wildfire-response platform**, enabling visual–language outputs for real-time validation.  
- Designed the interpretability layer to provide **descriptor-conditioned attention maps** for situational transparency and field operability.

---

## Key Findings

- **Descriptor fusion** significantly improves forecasting robustness under sparse or incomplete sensor data conditions.  
- The combination of **RGB–IR–textual modalities** enhances the model’s ability to capture both physical and contextual fire dynamics.  
- Integration within the Squishy Robotics platform demonstrates the framework’s applicability to **real-world autonomous response scenarios**, supporting mission planning and early warning systems.

---

## Acknowledgments

This research was conducted at the **Berkeley Expert Systems Technologies (BEST) Lab**, Department of Mechanical Engineering, UC Berkeley, in collaboration with **Squishy Robotics**.  
Supervised by **Dr. Alice Agogino** and supported by the **Wildfire Response Research Team**.
