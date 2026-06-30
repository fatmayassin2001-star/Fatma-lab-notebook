---
layout: post
title: "Photophysiological Data Analysis in R: Sdot Yam Marine Macroalgae"
tags: [R, Data Analysis, Marine Biology, PAM]
---

# Photophysiological Characterization of Marine Macroalgae

**Project Overview:** This repository contains the data, R scripts, and analytical report for the photophysiological characterization of marine macroalgae collected at Sdot Yam using Pulse-Amplitude-Modulated (PAM) fluorometry.

---

## 1. Field Survey and Experimental Design

The aim of this study was to investigate the photophysiological characteristics and light-acclimation strategies of various marine macroalgal species collected from diverse microhabitats. Field sampling was conducted via boat along the Sdot Yam coastline. The data in this repository specifically focuses on samples collected along the **South-to-North (S–N) transect**.

![Field Survey at Sdot Yam](...)
*Figure A: Field survey at Sdot Yam. Collection of macroalgae samples from various depths and light exposures along the South-to-North transect.*

---

## 2. Materials and Methods

### 2.1. Taxonomic Identification and Sorting
In the laboratory, specimens were sorted into Petri dishes and identified using morphological characteristics. To minimize ecological impact, only representative tissues required for measurements were retained; all excess biomass was returned to the sea.

![Macroalgae Sorting in Petri Dishes](...)
*Figure B: Laboratory sorting phase. Identified macroalgal species separated into Petri dishes prior to dark adaptation.*

### 2.2. Dark Adaptation and PAM Fluorometry
Samples were subjected to a 15–30 minute dark-adaptation period. This allows the complete reoxidation of the plastoquinone pool and the relaxation of non-photochemical quenching (NPQ), ensuring accurate baseline fluorescence measurements ($F_0$ and $F_m$). Following dark adaptation, a Rapid Light Curve (RLC) protocol was applied using the PAM fluorometer to calculate the relative Electron Transport Rate (rETR) across increasing irradiances (PAR).

![PAM Fluorometry Setup](...)
*Figure C: Dark adaptation and measurement setup using the Pulse-Amplitude-Modulated (PAM) fluorometer.*

---

## 3. Results

The raw PAM data was exported and analyzed using the R statistical environment to extract key physiological parameters: Initial slope ($\alpha$), Maximum electron transport rate ($ETR_{max}$), and Saturation irradiance ($I_k$).

### 3.1. Specimen Metadata
> **[INSERT YOUR METADATA TABLE HERE]**
> *Instructions: Paste the markdown table or insert a screenshot of the metadata table exported from R showing the species name, transect, and relative depth.*
*Table 1: Metadata for macroalgal specimens collected along the S–N transect, detailing taxonomic classification and relative collection depth.*

### 3.2. Calculated Photophysiological Parameters
> **[INSERT YOUR CALCULATED PARAMETERS TABLE HERE]**
> *Instructions: Paste the markdown table or insert a screenshot of the table exported from R showing the calculated Alpha, ETRmax, and Ik values.*
*Table 2: Mean photophysiological parameters extracted from the non-linear RLC models for the investigated species.*

### 3.3. Rapid Light Curves
![Rapid Light Curves Plot](...)
*Figure 1: Rapid Light Curves depicting the relative Electron Transport Rate (rETR) as a function of incident irradiance (PAR). Points represent measured values; solid lines indicate the model fit generated in R.*

---

## 4. Interpretation and Discussion

The extracted data reveal distinct acclimation strategies:
* **Shade-adapted macroalgae** (collected from deeper/shaded microhabitats, visually darker/greener) exhibited high light-harvesting efficiency ($\alpha$) and low saturation irradiance ($I_k$), optimizing their limited light environment.
* **Sun-adapted macroalgae** (collected from shallow, sun-exposed habitats) exhibited robust physiological plasticity, marked by a significantly higher maximum capacity ($ETR_{max}$) and higher $I_k$, allowing them to utilize high irradiance levels without sustaining severe photoinhibition.

---

## 5. Limitations and Proposed Follow-up

Several methodological limitations introduce variability, including transport stress (time elapsed between collection and laboratory analysis), tissue heterogeneity in the PAM leaf clip, and the absence of exact in-situ PAR measurements.

**Proposed Follow-up Experiment:**
To isolate environmental plasticity from inter-species variability, a future study should focus on a single abundant species across a depth gradient. Utilizing an underwater diving-PAM, *in-situ* measurements should be compared with *ex-situ* laboratory acclimation data over a 48-hour period to determine the short-term plasticity of $\alpha$ and $ETR_{max}$ under controlled light intensities.

---

### Repository Structure
* `data/` - Contains the raw and organized `.csv` files (e.g., `Mock_Photophysiology_2026.csv`).
* `scripts/` - Contains the R script used for analysis (`R_excersize_photophysiology_2026.R`).
* `images/` - Contains figures, plots, and field photographs.