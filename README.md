# Real-Power-System-Oscillation-Dataset

**Authors:**  
Yayu (Andy) Yang (yyang117@utk.edu), Hao Fu, Haozong Wang, Boming Liu

**Principal Investigator:** 
Jin Dong, Yilu Liu

**Affiliations:**  
- University of Tennessee, Knoxville, USA  
- Oak Ridge National Laboratory, USA

**Version:** 1.0  
**Release Date:** July 2026

---

## 1. Introduction
This dataset contains frequency measurement data for **11 oscillation events** collected across major power interconnections in continental North America, including: 
- Eastern Interconnection (EI), 
- Western Interconnection (WI), which is overseen in part by the Western Electricity Coordinating Council (WECC), and 
- Electric Reliability Council of Texas (ERCOT). 

The data is intended for researchers working on oscillation detection, modal analysis, and grid stability.

## 2. Dataset Specification
- **File Format:** CSV (.csv)
- **Reporting Rate:** 10 Hz (10 samples per second).
- **Data Structure:**
    - **Column 1:** UTC Time (Timestamp).
    - **Timestamp Format:** YYYY-MM-DD HH: MM: SS\.XXX (using XXX as milliseconds); 
    - **Columns 2 to N:** Frequency measurements from different PMU devices.
    - **Frequency Unit:** Hz
- **Interconnections Covered:** EI, WECC, and ERCOT.

## 3. PMU Identifier and Privacy Policy
To protect infrastructure-sensitive information, PMU channel names in the public release are anonymized and do not directly correspond to actual substations, utilities, or geographic identifiers.
- PMU channels are released using anonymized labels (e.g., PMU001, PMU002, ...).
- Relative oscillation characteristics and signal behaviors are preserved.
- Exact geographic metadata and utility ownership information are intentionally withheld in the public release.

This anonymization is intended to balance research usability with infrastructure security considerations.

## 4. Event Validation and Data Quality
The oscillation events included in this dataset were identified and cross-validated using multiple sources, including:
- NERC Technical Review Documents (TRD),
- FNET/GridEye disturbance observations,
- modal frequency analysis,
- and expert engineering review.

Dominant oscillation frequencies reported in this document are approximate modal estimates and may vary slightly depending on:
- preprocessing methods,
- analysis window selection,
- and modal estimation algorithms.

## 5. Event Summary Matrix
The table below lists the 11 events included in this open-source release along with their estimated dominant oscillation frequencies.

| Interconnection | Event ID (Date) | Dominant Frequency | Metadata Reference |
| :--- | :--- | :--- | :--- |
| **EI** | 2011-04-27 | 0.60 Hz | EI_OscillationEvent_20110427 |
| | 2019-01-11 | 0.24 Hz | EI_OscillationEvent_20190111 |
| | 2024-11-01 | 0.16 Hz | EI_OscillationEvent_20241101 |
| **WECC** | 2015-09-05 | 0.42 Hz | WECC_OscillationEvent_20150905 |
| | 2023-09-20 | 0.20 Hz | WECC_OscillationEvent_20230920 |
| | 2023-11-01 | 0.23 Hz | WECC_OscillationEvent_20231101 |
| | 2025-08-12 | 0.29 Hz | WECC_OscillationEvent_20250812 |
| **ERCOT** | 2025-02-08 | 0.50 Hz | ERCOT_OscillationEvent_20250208 |
| | 2025-04-25 | 0.50 Hz | ERCOT_OscillationEvent_20250425 |
| | 2025-04-28 | 0.50 Hz | ERCOT_OscillationEvent_20250428 |
| | 2025-09-09 | 0.50 Hz | ERCOT_OscillationEvent_20250909 |

## 6. Data Preprocessing Notes
- All timestamps are synchronized in Coordinated Universal Time (UTC).
- Frequency measurements are quality-checked prior to release.
- The released event segments were selected to maintain data completeness and consistency whenever possible.
- Unless otherwise stated, no additional oscillation-enhancement filtering or modal preprocessing is applied to the released data.

Researchers are encouraged to apply preprocessing methods appropriate for their specific analysis objectives.

## 7. Recommended Research Applications
This dataset is intended for:
- Oscillation detection,
- Modal frequency estimation,
- Benchmarking signal processing algorithms,
- Machine learning model development,
- Wide-area monitoring research,
- Power system stability studies.

The dataset is intended for research and educational purposes only and is not designed for operational decision-making without additional validation.

## 8.  Download
**[➡️ Download the Latest Release (V1)](https://github.com/yayuyang/PVSizer_Tool_AlphaVersion/releases)**

## 9. Project Funding

This work was supported by the **U.S. Department of Energy (DOE)** under the project:

**Solar Grid Integration Data Library and Model Validation Platform (OEDI SI II, 52746)**  

**Collaborating Institutions and Organizations**: 
- University of Tennessee
- Oak Ridge National Laboratory(ORNL)
