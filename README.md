# 14 nm FinFET Process Flow Simulation with Coventor Simulator 3D

**Author:** Stephen Singh  
**Affiliation:** Herbert Wertheim College of Engineering, University of Florida  
**Contact:** stephensingh953@gmail.com  

---

## Abstract

This project documents the detailed **process flow** for fabricating a 14 nm FinFET transistor, simulated end-to-end using **Coventor Simulator 3D**. Each major processing step—from wafer preparation through metallization—is described with emphasis on deposition, lithography, and etching methods.

## Keywords

FinFET • Etching • Deposition • RIE • Lithography • Coventor Simulator 3D

---

## Table of Contents

- [Abstract](#abstract)  
- [Keywords](#keywords)  
- [Introduction](#introduction)  
- [Step 1: Wafer Setup](#step-1-wafer-setup)  
  - [1.1 Silicon Foundation](#11-silicon-foundation)  
- [Step 2: Front End of Line (FEOL)](#step-2-front-end-of-line-feol)  
  - [2.1 Fins](#21-fins)  
  - [2.2 Fin Cuts](#22-fin-cuts)  
  - [2.3 Wells](#23-wells)  
  - [2.4 Shallow Trench Isolation (STI)](#24-shallow-trench-isolation-sti)  
  - [2.5 Gates](#25-gates)  
  - [2.6 Source and Drain](#26-source-and-drain)  
  - [2.7 Replacement Metal Gates (RMG)](#27-replacement-metal-gates-rmg)  
- [Step 3: Middle of Line (MOL)](#step-3-middle-of-line-mol)  
- [Conclusion](#conclusion)  
- [References](#references)  

---

## Introduction

Advanced transistor nodes such as 14 nm FinFET require extremely precise process integration. This simulation uses Coventor 3D to model:

- **Front-End-of-Line (FEOL)**: fin formation, gate wrap, source/drain engineering  
- **Middle-of-Line (MOL)**: contact metallization and trench fill  
- **Back-End-of-Line (BEOL)** steps are implied but not detailed here  

---

## Step 1: Wafer Setup

### 1.1 Silicon Foundation

Begin with a polished **silicon wafer block** as the substrate. Coventor simulates:

- Native oxide cleaning  
- Surface preparation to establish a defect-free starting plane  


---

## Step 2: Front End of Line (FEOL)

The FEOL encompasses all transistor-defining steps:

### 2.1 Fins

- **Layer stack depositions**: oxide, nitride, ODL, ARC, and photoresist  
- **Mandrel patterning** using **lithography** and **RIE**  
- **Spacer formation** and final fin release  


### 2.2 Fin Cuts

- Precision **RIE** etching to achieve target fin height (≈155 nm) and pitch (≈120 nm)  
- Removal of mandrel materials  


### 2.3 Wells

- **N- and P-well** implants simulated via rapid thermal processing (RTP)  
- Oxide/nitride masking and selective etch  


### 2.4 Shallow Trench Isolation (STI)

- HDP deposition and **CMP** planarization  
- RIE & wet clean to isolate adjacent devices  


### 2.5 Gates

- **Self-aligned contact oxide/silicon (SAC)** and gate cap stack deposition  
- **Gate wrap** around fins via lithography → RIE → wet clean  
- Final gate height ≈315 nm  


### 2.6 Source and Drain

- **Spacer oxide/nitride** deposition → lithography → RIE → wet clean  
- Epitaxy (EPI) fill with SiGe for PSD, SiC for NSD to tune electrical properties  



### 2.7 Replacement Metal Gates (RMG)

- Sacrificial gate removal  
- High-k dielectric + metal liner depositions (TiN, TaN)  
- CMP & RIE to form final metal gate trench  


---

## Step 3: Middle of Line (MOL)

- **Contact silicide** deposition (Ti, TiN, W)  
- **CMP** planarization and contact plug fill  
- Ensures low-resistance interconnects  


---

## Conclusion

This Coventor 3D simulation captures the intricacies of 14 nm FinFET process flow. Future work may extend to BEOL routing and statistical variability analysis.

---

## References

1. “14 nm lithography process,” WikiChip.  
2. Nikon, “Semiconductor Lithography Systems.”  
3. ASM, “Epitaxy.”  
