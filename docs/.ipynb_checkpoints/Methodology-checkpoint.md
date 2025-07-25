# **Methodology of the Normalized Radar Burn Ratio (NRBR)**

## **Overview**

The **Normalized Radar Burn Ratio (NRBR)** is a novel SAR-based index derived from Sentinel-1 C-band Synthetic Aperture Radar (SAR) data, designed to enhance burned area mapping by capturing fire-induced structural and dielectric changes in vegetation. The NRBR leverages the complementary responses of **VV** (Vertical transmit-Vertical receive) and **VH** (Vertical transmit-Horizontal receive) polarizations to improve detection accuracy across diverse land cover types.

#### 1. **Equation**

The NRBR is calculated as follows:

$$
NRBR = \frac{RBR_{VH} - RBR_{VV}}{RBR_{VH} + RBR_{VV}}
$$

Where:

- \\(RBR_{VV}\\) and \\(RBR_{VH}\\) are the Radar Burn Ratios for VV and VH polarizations, respectively, computed as the ratio of post-fire to pre-fire backscatter coefficients (\\(\sigma^0\\)) in power units.

#### 2. **In-depth understanding**

Burned areas generally exhibit reduced vegetation biomass and altered soil moisture, which influence the backscatter signal of **VV** and **VH** polarizations. The idea behind the **NRBR** is based on the fact that when vegetation is burned, the leaves are removed and the prevalent scattering structure is vertically oriented due to the presence of remaining stems and branches, the latter being particularly relevant for C-band scattering. This vertical structure contributes to the increased returns in burned areas than unburned areas for the VV polarization as the attenuating layer (leaves) is removed. For the **VH** polarization, which is more sensitive to volumetric dispersion and thus the tridimensional structure of the forest, the burned areas exhibit lower return power than the unburned areas. Therefore, **NRBR** may improve the contrast between burned and unburned areas (Fig. 3) with burned scars showing negative values and areas of no change showing positive values. This conceptualization of the **NRBR** index is in line with other optical indices such as Normalized Burn Ratio (NBR) or Normalized Difference Vegetation Index (NDVI).

Let us consider the following illustration as an example: for a burned area, the \\(RBR_{VH}\\) values will be less than 1, so the numerator \\(RBR_{VH}-RBR_{VV}<0\\) (negative), and the denominator \\(RBR_{VH}+RBR_{VV}>0\\) (positive). Therefore, the division \\(RBR_{VH}-RBR_{VV}/RBR_{VH}+RBR_{VV}\\) will compute substantially negative values for burned areas. This same reasoning applies to unburned areas, where \\(RBR_{VH}>1\\) and \\(RBR_{VV}<1\\), so that the numerator \\(RBR_{VH}-RBR_{VV}>0\\), divided by the denominator \\(RBR_{VH}+RBR_{VV}\\), will result in computing unburned areas with positive values.

<div style="text-align: center;">
  <img src="https://raw.githubusercontent.com/yotarazona/deeplearning_landcover/main/image/Fig3-modified.jpg" width="700"/>
</div>

#### 3. **Interpretation**

- **Negative values**: Indicate burned areas due to reduced \\(RBR_{VH}\\) (loss of volumetric scattering) and increased \\(RBR_{VV}\\) (enhanced backscatter from exposed vertical structures).
- **Positive values**: Represent unburned or unchanged areas.

#### 4. **Key Highlights**

The NRBR index mitigates common SAR limitations such as *speckle noise* and *topographic effects*. By computing pre- and post-fire backscatter differences, **NRBR** reduces i) random speckle in a manner similar to multi-temporal filtering and ii) because both pre- and post-fire acquisitions are equally affected by topography, their ratio used cancels out topographic influences, removing the need for additional terrain normalization procedures.

## **Advantages over other indices**

- **Robustness to Atmospheric Conditions**: Unlike optical indices (e.g., dNBR), NRBR is unaffected by clouds, smoke, or solar illumination, making it ideal for fire monitoring in persistently cloudy regions.
- **Topographic and Speckle Noise Mitigation**: Temporal ratios minimize terrain-induced distortions and speckle noise inherent in SAR data.
- **Dual-Polarization Sensitivity**: Combines VV (sensitive to vertical structures) and VH (sensitive to canopy volume), enhancing discrimination of burned areas across forests, shrublands, grasslands, etc.
- **All-Weather/Day-Night Capability**: Enables continuous monitoring, unlike optical sensors that rely on clear-sky conditions.

## **Performance in cloud-prone regions**

**NRBR** excels in cloud-affected areas where optical data (e.g., Sentinel-2/Landsat) are often unavailable. Studies demonstrate its reliability in Mediterranean and temperate ecosystems, achieving:

- **Dice Coefficient (DC)**: Up to 89.6% in forests and 84.2% in grasslands, outperforming dNBR in cloud-obscured regions.
- **Intersection over Union (IoU)**: Reaches 81.1% (Portugal) and 72.7% (Spain), with lower omission errors compared to optical methods.

## **Integration with Deep Learning**

The **NRBR** is integrated into a **U-Net architecture** for semantic segmentation, trained on 256×256-pixel patches. Key enhancements include:

- **Late Fusion**: Combines **NRBR** and **dNBR** probabilistic outputs to reduce errors (e.g., CE < 5%, OE < 12%).
- **Scalability**: Implemented in Google Earth Engine and TensorFlow, enabling global, near-real-time applications.

## **Broader Applications**

Beyond burned area mapping, **NRBR** shows potential for:

- **Fire severity assessment**: Correlates with optical indices (dNBR, dNDVI).
- **Post-fire recovery monitoring**: Tracks vegetation regrowth via temporal backscatter trends.
- **Disturbance mapping**: Detects deforestation or agricultural changes under cloud cover.

## **Conclusion**

The **NRBR** represents a significant advancement in SAR-based wildfire monitoring, offering a cloud-resilient, high-accuracy alternative to optical indices. Its integration with deep learning and multi-sensor fusion (Sentinel-1/2) provides a scalable solution for global burned area mapping, particularly in challenging environments.

<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>