# Water Scarcity Forecasting Using Machine Learning and Deep Learning

This repository presents the models developed during my Master's Thesis:  
**"Combining Process-Based and Data-Driven Approaches to Detect Drivers and Project Changes in Blue Water Scarcity"**,  
Politecnico di Milano, Laurea Magistrale in Environmental and Land Engineering (2024–2025).

Global freshwater resources face mounting pressure from climate change, population growth, and industrial expansion.
While traditional hydrological models provide accurate assessments of water scarcity, they are often computationally intensive and difficult to scale.
This project proposes a machine learning framework to efficiently forecast Blue Water Scarcity (BWS) by integrating sectoral water demand, geospatial features, and climate variables.

This work proposes a machine learning framework to forecast **Blue Water Scarcity (BWS)** efficiently using Hydrological Model results and combining sectoral water demand, geospatial features, and climatic variables.

The project aims to deliver an accurate, scalable, and computationally efficient tool for Hydrological Model to support adaptive and sustainable water management strategies.

---

## Models Developed

### LightGBM Model
- Features: sectoral water demand, 3D Cartesian coordinates converted, seasonal encodings, temperature, and precipitation.
- **Performance**:
  - **Nash-Sutcliffe Efficiency (NSE)**: 0.826
  - **Normalized Mean Squared Error (NMSE)**: 0.174
  - **Percent Bias (PBIAS)**: +4.398%

### Convolutional Neural Network (CNN)
- Features: structured grid inputs with multi-channel water demand and geospatial data.
- **Performance**:
  - **Nash-Sutcliffe Efficiency (NSE)**: 0.531
  - **Normalized Mean Squared Error (NMSE)**: 0.469
  - **Percent Bias (PBIAS)**: –2.874%

The LightGBM model consistently outperformed the CNN in terms of predictive accuracy and generalization.

---

## Repository Contents

- `LightGBM_Model.ipynb` — Full pipeline for LightGBM model development and evaluation.
- `CNN_Model.ipynb` — Deep learning model implementation and training.

---

## Data Sources

- Global monthly sectoral water withdrawal datasets (2010–2100) at 0.5° resolution.
- Climate data: temperature and precipitation projections based on SSP2–RCP4.5 scenarios, averaged over five Global Climate Models (GCMs).

---

## Main Findings

- Global blue water scarcity is projected to worsen significantly across South Asia, North Africa, and the Americas.
- Machine learning methods, especially LightGBM, can dramatically give the scalability and efficiency prediction of water scarcity.
- The proposed framework supports data-driven water governance and long-term planning under future climatic uncertainties.
