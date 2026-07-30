# Probabilistic State Parameter-Based Liquefaction Triggering Model

**Software, data, and documentation for a probabilistic liquefaction-triggering model formulated in state-parameter space.**

> **Publication status:** Accepted for publication in the  
> *ASCE Journal of Geotechnical and Geoenvironmental Engineering*.

---

## Overview

This repository contains the software, data, and documentation associated with the article:

***“Probabilistic State Parameter-Based Liquefaction Triggering Model”***

**Authors:** Pedro Reyes, Gonzalo Montalva, Vicente San Martín, and Robb Moss.

The proposed framework combines a laboratory-derived cyclic resistance model, **CRR(ψ)**, with Monte Carlo propagation of:

- CPT-derived state parameter, **ψ**, estimated using a Plewes-type procedure.
- Probabilistic seismic demand, **CSR**.
- Model and input uncertainties.

The workflow produces depth-dependent estimates of the probability of liquefaction, **P<sub>L</sub>**.

---

## Liquefaction Triggering Model

### Main file

[`CPT_to_PL.zip`](CPT_to_PL.zip)

This package reproduces the CPT-based probabilistic workflow used in the liquefaction-triggering study.

The cyclic resistance relationship, **CRR(ψ)**, is combined with Monte Carlo uncertainty propagation to calculate:

- Cone resistance, **q<sub>c</sub>**.
- Friction ratio, **R<sub>f</sub>**.
- Soil behavior type index, **I<sub>c,RW</sub>**.
- State parameter, **ψ**.
- Cyclic resistance ratio, **CRR(ψ)**.
- Probability of liquefaction, **P<sub>L</sub>**.

All results are presented as a function of depth.

---

## How to Use the Model

### 1. Prepare the working directory

Set the working directory to the folder containing the following files:

```text
CPT.xlsx
CRR_model.RData
CSR_model.RData
PSI_uncertainty.RData
