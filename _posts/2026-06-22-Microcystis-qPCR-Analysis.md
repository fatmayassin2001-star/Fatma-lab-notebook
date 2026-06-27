---
layout: post
title: "qPCR Experimental Design Analysis"
---
#  qPCR Experimental Design & Relative Quantification Analysis

**Objective:** To establish a molecular tracking protocol detecting the genetic potential of taste and odor (T&O) compound production under environmental stress, and to analyze relative gene expression data using the comparative Ct method.

---

# Part 1: Experimental Design

Experimental Overview
* Chosen Organism: *Microcystis* (e.g., *Microcystis aeruginosa*)
* Experimental Stressor: Elevated water temperature combined with nutrient stress (e.g., altered N:P ratio) to simulate seasonal transitions and algal bloom triggers.
* Control Group: Cultures maintained under optimal growth conditions without heat or nutrient stress, serving as the baseline for comparison.
* Experimental Rationale: Elevated temperature and nutrient imbalance are among the primary environmental drivers of cyanobacterial blooms. These conditions are frequently associated with increased production of taste-and-odor compounds in freshwater systems, making them biologically relevant stressors for this study.

Target Genes Selection

**1. *geoA***
* Biological Function: Encodes geosmin synthase (converts FPP into geosmin, causing earthy/musty odors).
* Expected Observation: Upregulation.
* Relevance to Stress: Stress responses trigger metabolic shifts. Overexpression precedes detectable chemical outbreaks, serving as an early-warning marker.

**2. *mic***
* Biological Function: Encodes 2-methylisoborneol synthase (synthesizes 2-MIB, causing severe musty odors).
* Expected Observation: Upregulation.
* Relevance to Stress: Expression correlates tightly with active growth phases and heat/nutrient stress, quantifying the genetic potential for nuisance compounds.

## Reference (Housekeeping) Gene

**rpoC1**
* Biological Function: Encodes the RNA polymerase gamma subunit.
* Justification for Stability: Essential for basal transcription and cell viability. It exhibits constitutive expression, remaining highly stable across environmental fluctuations for accurate normalization.

## Hypothesis
Elevated temperature and nutrient stress are expected to increase the expression of geoA and mic genes in Microcystis, reflecting an increased genetic potential for geosmin and 2-MIB production. In contrast, the reference gene rpoC1 is expected to remain stable because it is involved in essential cellular transcription processes.

---

## Part 2: Data Interpretation (ΔΔCt Method)

**Calculation Workflow (Livak ΔΔCt Method)**
To analyze the relative fold change in gene expression between the **Inhibitor Treatment** and **DMSO Control**, we utilize the comparative Ct method.

1. **Normalization (ΔCt):** Corrects for differences in input amount and RNA quality. 
> ΔCt = Ct (Target) - Ct (Reference Gene)

2. **Relative Difference (ΔΔCt):** Compares treatment against the control baseline.
> ΔΔCt = ΔCt (Treatment) - ΔCt (Control)

3. **Fold Change:** Determines the final expression ratio. > Fold Change = 2<sup>-ΔΔCt</sup>
---

# 📈 Data Visualization

*(Below is the visual representation of the calculated Fold Changes comparing the Inhibitor treatment vs. DMSO Control)*

![alt text](../images/image-1.png)

## 💡 Final Conclusion
The relative quantification analysis suggests that the inhibitor produces a selective transcriptional response rather than a global cellular shutdown. It successfully represses targeted developmental genes (such as pitx and sm50) while simultaneously triggering a distinct stress or compensatory response in the NGN and soxC pathways.
