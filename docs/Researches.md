# 🔬 Researches on NRBR Index

## 📄 Normalized Radar Burn Ratio: A Case Study for Burned Area Mapping in Mediterranean Forests

**Summary**  
This foundational research introduces the Normalized Radar Burn Ratio (NRBR)—a new index that combines RBR_VV and RBR_VH from Sentinel-1 to enhance burned area detection. Tested with U-Net over 2017 fires in Portugal, NRBR showed higher accuracy and less omission error than traditional radar indices, and correlated strongly with NDVI (Normalized Difference Vegetation Index) and dNBR (delta Normalized Burn Ratio).

**Highlights**  
- 🌍 Region: Meditarranean forest  
- 🛰️ Data: Sentinel-1 VV/VH polarizations  
- 🤖 Model: U-Net, 512×512 patches  
- 📈 Accuracy: Omission Error = 19% (vs. 32–66% for other indices)  
- 🔍 Insight: Strong correlation with NDVI and dNBR (r > 0.7)

**Citation**  
*Tarazona, Y., Tanase, M.A., & Mantas, V. M. (2025). **Normalized Radar Burn Ratio: A Case Study for Burned Area Mapping in Mediterranean Forests**, IEEE Geoscience and Remote Sensing Letters., 2025. In review.*

---

## 📄 Combining Ascending and Descending Sentinel-1 modes for Enhancing burned area mapping with Normalized Radar Burn Ratio

**Summary**  
This foundational research introduces the Normalized Radar Burn Ratio (NRBR)—a new index that combines RBR_VV and RBR_VH from Sentinel-1 to enhance burned area detection. Tested with U-Net over 2017 fires in Portugal, NRBR showed higher accuracy and less omission error than traditional radar indices, and correlated strongly with NDVI (Normalized Difference Vegetation Index) and dNBR (delta Normalized Burn Ratio).

**Highlights**  
- 🌍 Region: Meditarranean forest  
- 🛰️ Data: Sentinel-1 VV/VH polarizations  
- 🤖 Model: U-Net, 512×512 patches  
- 📈 Accuracy: Omission Error = 19% (vs. 32–66% for other indices)  
- 🔍 Insight: Strong correlation with NDVI and dNBR (r > 0.7)

**Citation**  
*Tarazona, Y., & Mantas, V. M. (2025). **Combining Ascending and Descending Sentinel-1 modes for Enhancing burned area mapping with Normalized Radar Burn Ratio**, Presented at Living Planet Symposium 2025. Zenodo. [https://doi.org/10.5281/zenodo.15766613](https://doi.org/10.5281/zenodo.15766613)*.

---

## 📄 Advancing Burned Area Mapping using the Normalized Radar Burn Ratio (NRBR)

**Summary**  
This study evaluates the NRBR’s sensitivity to post-fire changes across land cover types (forest, shrub, grassland) using Sentinel-1 and U-Net segmentation. Compared to dNBR, NRBR performs better in grasslands (IoU = 57.6% vs. 53.4%) and comparably in forests, indicating strong potential for SAR-based burned area mapping under cloudy conditions.

**Highlights**
- 🌍 Region: Portugal (2017 fires)
- 🛰️ Data: Sentinel-1 (C-SAR) vs. Sentinel-2 (dNBR)
- 🤖 Model: U-Net, 512×512 patches
- 📈 Accuracy: Dice (Forest) = 79.3%, Dice (Grassland) = 73.0%
- 📌 Insight: NRBR complements optical indices in mixed land covers

**Citation**  
*Tarazona, Y., Tanase, M.A., & Mantas, V. M. (2025). **Normalized Radar Burn Ratio: A Case Study for Burned Area Mapping in Mediterranean Forests**, IEEE Geoscience and Remote Sensing Letters., 2025. In review.*

---

## 📄 Scalable Burned Area Mapping via Sentinel-1/2 Fusion using the new NRBR Index

**Summary**  
This study presents the first cross-continental assessment of the NRBR index, derived from dual-polarized Sentinel-1 data, for burned area detection in Portugal, Spain, and California. Using U-Net segmentation and a late-fusion strategy with dNBR (Sentinel-2), the model achieved up to **91.9% Dice Coefficient** and **85.1% IoU**, surpassing individual sensors. Implemented entirely in **Google Earth Engine and TensorFlow**, this work demonstrates the **scalability and robustness** of NRBR for operational fire mapping across diverse landscapes and atmospheric conditions.

**Highlights**
- 🌍 Regions: Portugal, Spain, California
- 🛰️ Data: Sentinel-1 VV/VH + Sentinel-2 (dNBR)
- 🤖 Model: U-Net, 256×256 patches, late fusion
- 📈 Accuracy: Dice = 91.9%, IoU = 85.1%
- ☁️ Application: Robust performance under cloud/smoke

**Citation**  
*Tarazona, Y., Tanase, M.A., & Mantas, V. M. (2025). **Normalized Radar Burn Ratio: A Case Study for Burned Area Mapping in Mediterranean Forests**, IEEE Geoscience and Remote Sensing Letters., 2025. In review.*

---
