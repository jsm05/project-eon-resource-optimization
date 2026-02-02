# Project eON – Eco-Optimization Nexus

## Overview
Project eON is a data-driven sustainability prototype designed to extend the usable lifespan of smartphones by optimizing software-level resource usage. The project addresses premature device replacement caused by software inefficiencies rather than actual hardware failure.

The system combines exploratory data analysis, interpretable machine learning, and client-side inference to demonstrate how intelligent software optimization can reduce battery degradation, system lag, and unnecessary background activity.

---

## System Architecture
Project eON follows a three-stage, MLOps-inspired pipeline:

### Stage 1: Exploratory Data Analysis (Diagnosis)
- Analysis of large-scale smartphone process logs
- Parsing and explosion of nested JSON app data
- Temporal usage pattern discovery
- Identification of background-heavy and battery-draining applications

### Stage 2: Model Training (Intelligence Extraction)
- Rule-based intelligence model trained on cleaned usage data
- Timezone normalization to preserve behavioral patterns
- Threshold-based filtering to remove noise
- Learned temporal usage patterns exported as a structured model

### Stage 3: Client-Side Deployment (Inference & Verification)
- Lightweight web-based prototype using HTML, CSS (Tailwind), and JavaScript
- Client-side inference with no backend dependency
- Real-time decision visualization and user override controls
- Live MLOps-style verification interface

---

## Key Design Principles
- **Interpretability-first ML**: All decisions are traceable to learned usage patterns
- **Separation of concerns**: Training, inference, and UI logic are clearly isolated
- **User agency**: Model recommendations can be explicitly overridden
- **Privacy-aware deployment**: No device data leaves the client

---

## Tech Stack
- Python (pandas, matplotlib)
- Jupyter / Google Colab
- HTML5, CSS (Tailwind)
- Vanilla JavaScript

---

## Dataset
- The project uses a cleaned subset (~20,677 rows) of an academic smartphone usage dataset.
- The original dataset is intentionally not included due to size constraints.
- All preprocessing, feature extraction, and model logic are fully contained in the notebooks.

---

## How to Run
1. Open `notebooks/eon_eda.ipynb` to explore the data analysis.
2. Run `notebooks/eon_model_training.ipynb` to generate the trained usage model.
3. Open `web/index.html` in a browser.
4. Interact with each stage to observe model recommendations and system behavior.

---

## What This Project Demonstrates
- Systems engineering applied to sustainability
- Rule-based machine learning for behavioral modeling
- Client-side ML inference without cloud infrastructure
- Transparent, user-controllable optimization logic

---

## Authors
Jashan Singh Mehta
Kushagra Agrawal
