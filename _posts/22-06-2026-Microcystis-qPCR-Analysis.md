---
layout: post
title: "qPCR Experimental Design Analysis"
---

# qPCR Experimental Design & Relative Quantification Analysis

**Objective:** To establish a molecular tracking protocol detecting the genetic potential and metabolic pathways of taste and odor (T&O) compound production, and to analyze relative gene expression data using the comparative Ct method.

---

## Part 1: Experimental Design

**Experimental Overview**
* **Chosen Organism:** *Microcystis* (e.g., *Microcystis aeruginosa*)
* **Primary Focus:** Characterization of the genetic potential and metabolic pathways driving T&O production, prioritizing internal metabolic shifts rather than relying on physico-chemical stressors as primary drivers.

**Target Genes Selection**

**1. *geoA***
* **Biological Function:** Encodes geosmin synthase (converts FPP into geosmin, causing earthy/musty odors).
* **Expected Observation:** Upregulation.
* **Relevance:** Overexpression precedes detectable chemical outbreaks, serving as a direct marker for metabolic pathway activation.

**2. *mic***
* **Biological Function:** Encodes 2-methylisoborneol synthase (synthesizes 2-MIB, causing severe musty odors).
* **Expected Observation:** Upregulation.
* **Relevance:** Quantifies the genetic potential for nuisance compounds during active growth phases.

### Reference (Housekeeping) Gene

***rpoC1***
* **Biological Function:** Encodes the RNA polymerase gamma subunit.
* **Justification for Stability:** Essential for basal transcription and cell viability. It exhibits constitutive expression, remaining highly stable for accurate normalization.

---

## Part 2: Data Interpretation (ΔΔCt Method)

**Calculation Workflow (The Livak Method)**
To analyze the relative fold change in gene expression between the **Inhibitor Treatment** and **DMSO Control**, we utilize the comparative Ct method.

1. **Normalization (ΔCt):** Corrects for differences in input amount and RNA quality.
   > ΔCt = Ct (Target) - Ct (Reference Gene)

2. **Relative Difference (ΔΔCt):** Compares treatment against the control baseline.
   > ΔΔCt = ΔCt (Treatment) - ΔCt (Control)

3. **Fold Change:** Determines the final expression ratio.
   > Fold Change = 2<sup>-ΔΔCt</sup>

---

## Experimental Findings
*(Reference Gene Used: Tubulin, Ct ≈ 23.29)*

| Regulatory Response | Identified Genes | Calculated Fold Change | Biological Conclusion |
| :--- | :--- | :--- | :--- |
| **Severe Downregulation** | `pitx`, `sm50`, `SM30` | 0.24, 0.46, 0.57 | The inhibitor acts as a potent repressor of these specific developmental pathways. |
| **Notable Upregulation** | `NGN`, `soxC` | 1.99, 1.67 | The treatment triggers an overexpression or stress-compensatory induction in these targets. |
| **Negligible Change** | `synB`, `pak3` | 1.04, 1.07 | Pathways remain unaffected, demonstrating the high specificity of the inhibitor. |

---

## 📈 Data Visualization

*(Below is the visual representation of the calculated Fold Changes comparing the Inhibitor treatment vs. DMSO Control)*

![Data Visualization of Fold Changes](/image-1.png)

## 💡 Final Conclusion
The quantitative analysis demonstrates that the inhibitor is highly specific, generating a divergent regulatory response rather than a systemic cellular shutdown. It successfully represses targeted developmental genes while simultaneously triggering a distinct stress or compensatory response in the *NGN* and *soxC* pathways.