# BMEN 600 Project — Group 19
**Authors:** Chelsea Taylor, Gillian Twible, Jerold Lukaszuk, Michael Cuch  
**Date:** November 26, 2026  

## Research Question
How do longitudinal changes in the median frequency of uterine EHG signals between approximately 23 and 31 weeks of gestation differ among pregnancies resulting in induced labour, cesarean delivery, or both, and which recording channels (S1–S4) demonstrate the greatest differences between groups?

---

## Dataset & Access Instructions
This project uses the **Icelandic 16-electrode Electrohysterogram Database (`icehg-ds`, v1.0.1)** hosted on PhysioNet:
* **Source URL:** https://www.physionet.org/content/icehg-ds/1.0.1/

### How to Access & Set Up the Data
1. Download the `icehg-ds` (version 1.0.1) files directly from PhysioNet (open-access dataset).
2. Upload the dataset folder to Google Drive at the following path:
   `/content/drive/MyDrive/BMEN 600/EHG Dataset/files/icehg-ds/1.0.1`
3. Pre-processed intermediate cohorts and extracted median frequency tables are also included directly in this repository under `data/` and `results/` so downstream analysis can be reproduced without re-downloading raw WFDB records:
   * excel files Table1_induced.xlsx, Table2_cesarean.xlsx, and Table3_induced_cesarean.xlsx were used to make the tables of filtered data in colab in the file Filtered_data.ipynb.

---

## Software & Setup Instructions
* **Platform:** Google Colab (Python 3.10+)
* **Required Packages:**
  * `numpy`
  * `pandas`
  * `wfdb` (for reading PhysioNet EHG signal headers and records)
  * `scipy` (signal filtering and statistical testing)
  * `matplotlib`
