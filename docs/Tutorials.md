<!-- #region -->
# **Tutorials**

Welcome to the practical hub for the Normalized Radar Burn Ratio (NRBR). This page hosts a collection of interactive tutorials and Jupyter Notebooks designed to help researchers, analysts, and students understand, compute, and apply the NRBR index with real satellite data.

#### Why These Tutorials?

- 🛠️ From Theory to Code: Bridge the gap between the scientific paper and operational use. Each notebook translates a key methodological step into executable code.
- 🌍 Work with Real Data: All tutorials are designed to work with real Sentinel-1 SAR data from actual wildfire events.
- ⚡ Accelerate Your Research: Use our pre-configured code examples as a template for your own analysis of fire-affected regions anywhere in the world.
- 🔍 Promote Transparency & Reproducibility: We believe in open science. These notebooks provide the complete computational workflow behind the NRBR index, allowing for full scrutiny and adaptation.

## Downloading NRBR

The application enables global-scale downloads of the Normalized Ratio Burn Ratio (NRBR) index, along with dNBR (differenced Normalized Burn Ratio) and pre- and post-fire Landsat optical imagery. Users can easily filter data by selecting a country of interest, followed by a specific state or department, and finally choosing the 100×100 km tiles that cover the desired region. 

<div style="text-align: center;">
  <a href="https://ee-geoyons.projects.earthengine.app/view/nrbr" target="_blank">
    <img src="https://raw.githubusercontent.com/yotarazona/deeplearning_landcover/main/image/gee_app.png" width="950"/>
  </a>
</div>


#### Tutorial Gallery

**Notebook 1: Your First NRBR Map**

- [Deep Learning Burned area Segmentation Using SAR Sentinel-1.ipynb](https://github.com/yotarazona/scikit-eo/blob/main/examples/notebooks/17_Deep_Learning_Burned_area_Segmentation_UsingRadar.ipynb)
  
**Notebook 2: Comparing NRBR with Optical Indices (dNBR)**

- [Deep Learning Burned area Segmentation Using Optical Sentinel-2.ipynb](https://github.com/yotarazona/scikit-eo/blob/main/examples/notebooks/18_Deep_Learning_Burned_area_Segmentation_UsingOptical.ipynb)

**Notebook 3: U-Net for Burned Area Mapping using NRBR — Part 1: Training on Large Areas**

- [DL_Unet_BA_Part1_LargeAreas_NRBR.ipynb](https://github.com/yotarazona/scikit-eo/blob/main/examples/notebooks/19_DL_Unet_BA_Part1_LargeAreas_NRBR.ipynb)
  
**Notebook 4: U-Net for Burned Area Mapping using NRBR — Part 2: Prediction & Mosaicking**

- [DL_Unet_BA_Part2_LargeAreas_NRBR.ipynb](https://github.com/yotarazona/scikit-eo/blob/main/examples/notebooks/20_DL_Unet_BA_Part2_LargeAreas_NRBR.ipynb)
