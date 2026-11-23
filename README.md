# Photovoltaic Cell Defect Localization and Area Quantification

**Xiaoyu Shang · Lisbon College, Shanghai University**  
Independent course project · April–June 2026

[View the project report (PDF)](./pv-el-report.pdf)

## Project overview

A bounding box can locate a crack in an electroluminescence (EL) image,
but much of the enclosed area may be healthy. This project uses pixel-level
segmentation to estimate how much of each photovoltaic cell is affected
and which defect types account for that area.

## Methods and results

- Compared YOLOv8n and YOLOv8s for defect localization. YOLOv8s achieved
  72.7% mAP@50.
- Used DeepLabV3-ResNet50 to segment four defect types: cracks, contact
  anomalies, interconnect anomalies, and corrosion.
- Calculated the fraction of each cell covered by each defect type.
  Cracks occupied 4.89% of cell area on average in the analyzed images.
- Combined the area fractions with predefined weights to score individual
  cells. The report also explores module-level power loss and EV charging
  supply risk under simulated conditions.
