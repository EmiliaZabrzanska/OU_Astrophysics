# 🔭 Time-Series Photometric Analysis of XO-2Nb

**Author:** Emilia Zabrzanska  
**Date:** April 2025  

This repository contains my analysis of the transiting exoplanet **XO-2Nb**, completed as part of the Open University S384 module. The project makes use of data obtained with the **PIRATE telescope** and reduced with the **HOPS pipeline** to generate a light curve and extract transit parameters.

---

## 📘 Project Overview

Transiting exoplanets are a cornerstone of modern astrophysics, allowing measurement of orbital properties, planetary radii, and even atmospheric composition.  

This project focuses on **XO-2Nb**, a hot Jupiter orbiting the K-dwarf XO-2N, itself part of a wide binary system where both stars host planets. XO-2Nb is well studied in literature, making it an ideal target for testing ground-based photometric methods.  

Using **time-series photometry**, I produced a high-quality light curve and fitted a transit model to extract key orbital and planetary parameters.

---

## 🎯 Objectives

- Reduce raw PIRATE telescope data using **bias correction, flat-fielding, alignment**.  
- Perform **differential photometry** using carefully selected comparison stars.  
- Fit the transit light curve using **MCMC methods in HOPS**.  
- Derive parameters such as:  
  - Orbital period (P)  
  - Mid-transit time (T<sub>mid</sub>)  
  - Radius ratio (Rp/R\*)  
  - Inclination (i)  
  - Scaled semi-major axis (a/R\*)  
- Compare results with published values from Burke et al. (2007), Sing et al. (2012), and Damasso et al. (2015).  

---

## 🧮 Methods

- **Observations**: 571 frames over 9.5 hours on 24 Jan 2025 with the PIRATE telescope (R filter, 50s exposures).  
- **Calibration**: Bias subtraction, flat-field correction, alignment.  
- **Photometry**: Ensemble differential photometry with comparison stars matched in brightness and colour.  
- **Transit fitting**: MCMC fitting in HOPS, detrending against airmass and systematics.  
- **Quality checks**: Autocorrelation analysis, rejection of poor-quality frames.  

---

## 📊 Results

- **Orbital period**:  
  P = 2.61585982 days (matches literature within microseconds).  

- **Mid-transit time**:  
  T<sub>mid</sub> = 2460700.47875 ± 0.00038 BJD.  

- **Inclination**:  
  i = 88.0° (consistent with near-central transit).  

- **Radius ratio**:  
  Rp/R\* = 0.1013 ± 0.0010 → Transit depth δ ≈ 1.26%.  

- **Planetary radius** (assuming R\* = 0.97 R⊙):  
  Rp ≈ 0.98 R<sub>Jup</sub>.  

✅ Results agree strongly with published values, confirming the reliability of PIRATE + HOPS for exoplanet studies.  

---

## ⚖️ Limitations

- Eccentricity fixed to zero (no radial velocity data in this project).  
- Single-band (R) photometry only.  
- No limb-darkening coefficients fitted.  
- Dependent on calibration quality and comparison star stability.  

---

## 📂 Repository Contents

- `S384_TMA03_Report.pdf` – Full project report (with figures, light curve, and discussion).  
- `README.md` – Project summary (this file).  
- *(Optional future additions: Jupyter notebooks or Python scripts for light curve analysis outside HOPS).*  

---

## 📚 References

- Burke et al. (2007). *XO-2b: Transiting Hot Jupiter in a Metal-rich Binary.* ApJ, 671, 2115–2128.  
- Sing et al. (2012). *Detection of sodium in XO-2b from differential spectroscopy.* MNRAS, 426, 1663–1670.  
- Damasso et al. (2015). *Comprehensive analysis of the XO-2 stellar and planetary systems.* A&A, 575, A111.  
- Narita et al. (2011). *Rossiter–McLaughlin effect in XO-2Nb.* PASJ, 63, L67.  

---

## 📬 Contact

- 📧 [emiliazabrzanska02@gmail.com](mailto:emiliazabrzanska02@gmail.com)  
- 💼 [LinkedIn – Emilia Zabrzanska](https://www.linkedin.com/in/emilia-zabrzanska/)  

---

## 📜 License

This project is shared under the **MIT License**.  
You are free to use, adapt, and cite this analysis with attribution.
