# Scalable burned area mapping via Sentinel-1/2 fusion

This repository is part of the article *"Scalable burned area mapping via Sentinel-1/2 fusion"* (Tarazona and Mantas, under review in *Remote Sensing of Environment*) and corresponds to Appendix A of the manuscript.

The study evaluates the Normalized Radar Burn Ratio (NRBR), derived from Sentinel-1 dual-polarized C-band SAR data, and the optical differenced Normalized Burn Ratio (dNBR), derived from Sentinel-2, across Mediterranean, chaparral and boreal ecosystems in Portugal, Spain, California and Canada. Independent U-Net models are trained on each index, and their probabilistic outputs are combined through a simple late-fusion (averaging) strategy. Using only two derived input variables, the fused model outperformed both single-sensor models in all test tiles, achieving Dice Coefficients of 87â€“92%. The full workflow is implemented in Google Earth Engine (GEE) and TensorFlow.

#### Reproducibility

- 🛰️ **Scene identifiers:** [GEE script to list the Sentinel-1 and Sentinel-2 scenes used per tile and pre-/post-fire window](LINK_TO_SCRIPT), reproducing the image counts reported in Table 1 of the manuscript.

---

# NRBR

Welcome to the practical hub for the Normalized Radar Burn Ratio (NRBR). This page hosts a collection of interactive tutorials and Jupyter Notebooks designed to help researchers, analysts, and students understand, compute, and apply the NRBR index with real satellite data.

#### Why These Tutorials?

- 🛠️ From Theory to Code: Bridge the gap between the scientific paper and operational use. Each notebook translates a key methodological step into executable code.
- 🌍 Work with Real Data: All tutorials are designed to work with real Sentinel-1 SAR data from actual wildfire events.
- ⚡ Accelerate Your Research: Use our pre-configured code examples as a template for your own analysis of fire-affected regions anywhere in the world.
- 🔍 Promote Transparency & Reproducibility: We believe in open science. These notebooks provide the complete computational workflow behind the NRBR index, allowing for full scrutiny and adaptation.

#### Tutorial Gallery

**Notebook 1: Your First NRBR Map**

- [Deep Learning Burned area Segmentation Using SAR Sentinel-1.ipynb](https://github.com/yotarazona/scikit-eo/blob/main/examples/notebooks/17_Deep_Learning_Burned_area_Segmentation_UsingRadar.ipynb)
  
**Notebook 2: Comparing NRBR with Optical Indices (dNBR)**

- [Deep Learning Burned area Segmentation Using Optical Sentinel-2.ipynb](https://github.com/yotarazona/scikit-eo/blob/main/examples/notebooks/18_Deep_Learning_Burned_area_Segmentation_UsingOptical.ipynb)