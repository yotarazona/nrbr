# 🔬 Researches on NRBR Index

## 📄 Normalized Radar Burn Ratio: A Case Study for Burned Area Mapping in Mediterranean Forests

**Summary**  
This research introduces the Normalized Radar Burn Ratio (NRBR), an index designed to enhance burned area detection using Sentinel-1 C-band radar imagery. The research utilizes post- to pre-fire ratios of VV and VH backscatter coefficient to compute the NRBR, optimizing thus the contrast between burned and unburned areas. The 2017 wildfires in Portugal were used to validate the methodology. Using the U-Net architecture the NRBR based model outperforms previous ratio-based indices in metrics such as overall accuracy, omission error and Intersection over Union, among other metrics. Additionally, high correlations (r> 0.7) between NRBR and the optical indices NDVI (post-fire) and dNBR were observed. This approach has promising implications for improving burned area mapping, particularly for periods with cloud cover or occlusion from fire smoke.

**Highlights**  
- 🌍 Region: Meditarranean forest  
- 🛰️ Data: Sentinel-1 VV/VH polarizations  
- 🤖 Model: U-Net, 512×512 patches  
- 📈 Accuracy: Omission Error = 19% (vs. 32–66% for other indices)  
- 🔍 Insight: Strong correlation with NDVI and dNBR (r > 0.7)

**Citation**  
*Tarazona, Y., Tanase, M.A., & Mantas, V. (2025). **Normalized Radar Burn Ratio: A Case Study for Burned Area Mapping in Mediterranean Forests**, IEEE Geoscience and Remote Sensing Letters., 2025. [https://doi.org/10.1109/LGRS.2025.3592093](https://doi.org/10.1109/LGRS.2025.3592093)*

---

## 📄 Combining Ascending and Descending Sentinel-1 modes for Enhancing burned area mapping with Normalized Radar Burn Ratio

**Summary**  
This study evaluates the Normalized Radar Burn Ratio (NRBR) for burned area mapping using Sentinel-1 SAR data, comparing ascending, descending, and combined acquisition modes of Sentinel-1. Results show that integrating both orbits significantly improves accuracy (0.921), recall (0.858), and reduces omission errors (14.2%), making NRBR a reliable tool for wildfire monitoring.

**Highlights**  
- 🌍 Region: Meditarranean forest  
- 🛰️ Data: Sentinel-1 VV/VH polarizations 
- 🤖 Model: U-Net, 512×512 patches  
- 📈 Accuracy: Omission Error = 14% (vs. 18-19% for other indices)

**Citation**  
*Tarazona, Y., & Mantas, V. (2025). **Combining Ascending and Descending Sentinel-1 modes for Enhancing burned area mapping with Normalized Radar Burn Ratio**, Presented at Living Planet Symposium 2025. Zenodo. [https://doi.org/10.5281/zenodo.15766613](https://doi.org/10.5281/zenodo.15766613)*.

---

## 📄 Advancing Burned Area Mapping using the Normalized Radar Burn Ratio (NRBR)

**Summary**  
This research evaluates the Normalized Radar Burn Ratio (NRBR) for burned area mapping across mainland Portugal, a representative Mediterranean climate region. Using Sentinel-1 C-band SAR data and a U-Net deep learning model, the study provides a regional-scale assessment of NRBR across different land cover types and compares its performance with the optical-based dNBR index derived from Sentinel-2. Results show that NRBR achieves performance comparable to dNBR, with particularly strong results in grassland-dominated landscapes. In forested areas, dNBR obtained higher accuracy, while in grasslands NRBR slightly outperformed dNBR. These findings highlight the potential of NRBR as a radar-based alternative or complement to optical approaches, especially when cloud cover, smoke, or atmospheric conditions limit the use of optical imagery.

**Highlights**  
- 🌍 Region: Continental Portugal, Mediterranean climate zone
- 🛰️ Data: Sentinel-1 VV/VH polarizations and Sentinel-2 dNBR
- 🤖 Model: U-Net, 512×512 patches  
- 📈 Accuracy: NRBR achieved IoU = 64.8% and Dice Coefficient = 79.3% in forested areas

**Citation**  
*Tarazona, Y., & Mantas, V. (2026). **Advancing burned area mapping using the Normalized Radar Burn Ratio (NRBR)**. Remote Sensing Applications: Society and Environment, 41, 101938. [https://doi.org/10.1016/j.rsase.2026.101938](https://doi.org/10.1016/j.rsase.2026.101938)*.

## 📄 The Impact of Radiometric Terrain Normalization (γ⁰) on Burned Area Mapping Accuracy Using Sentinel-1 data

**Summary**  
This study evaluates whether applying angular-based radiometric terrain normalization (RTN) improves burned area mapping using Sentinel-1 SAR data and the Normalized Radar Burn Ratio (NRBR). The research compares NRBR calculated from standard sigma nought (σ⁰) backscatter with NRBR calculated from gamma nought (γ⁰) corrected using an angular-based RTN model implemented in Google Earth Engine. Results show that RTN has a region-dependent effect. In Portugal, NRBR without RTN achieved better overall performance, suggesting that the correction may introduce overcorrection or additional inconsistencies in moderate terrain. In California, RTN slightly improved overall accuracy and Dice Coefficient while reducing commission errors, although omission errors remained high. The study concludes that RTN can improve SAR radiometric consistency, especially on backslopes, but does not necessarily improve burned area detection with NRBR because the index already reduces topographic effects through pre- and post-fire backscatter ratios.

**Highlights**  
- 🌍 Region: Portugal and California
- 🛰️ Data: Sentinel-1 VV/VH polarizations
- 🛰️ Method: Comparison between σ⁰-based NRBR and γ⁰-based NRBR with RTN
- 🤖 Model: U-Net, 512×512 patches  
- 📈 Accuracy: In Portugal, NRBR without RTN achieved OA = 0.949, IoU = 0.811 and DC = 0.896. In California, RTN improved DC from 0.680 to 0.737

**Citation** 

*Tarazona, Y., & Mantas, V. (2026). **The Impact of Radiometric Terrain Normalization (γ⁰) on Burned Area Mapping Accuracy Using Sentinel-1 data**. EGU General Assembly 2026, Vienna, Austria, 3–8 May 2026, EGU26-15290. [https://doi.org/10.5281/zenodo.18838440](https://doi.org/10.5281/zenodo.18838440)*.

---

## 📄 Scalable Burned Area Mapping via Sentinel-1/2 Fusion using the new NRBR Index

## 🚧 **Work in Progress**  
<img src="https://media.giphy.com/media/3oKIPEqDGUULpEU0aQ/giphy.gif" width="200" height="200"> *(Coming Soon!)*  

---
