# Hardware‑Centric Analysis of Analog FM and Digital PCM on the ETT‑101

A single‑document, experiment‑centric report for **Analog Frequency Modulation (FM)** and **Digital Pulse‑Code Modulation (PCM)** implemented on the **Emona ETT‑101** modular trainer. This README holds **all details in one place**—from objectives to procedures, data, analysis, results, QA, and references.

---

## Table of Contents
- [0. Overview](#0-overview)
- [1. Platform and Safety](#1-platform-and-safety)
- [2. Repository Pointers](#2-repository-pointers)
- [3. Experiment 01 — Frequency Modulation (FM)](#3-experiment-01--frequency-modulation-fm)
  - [3.1 Objective](#31-objective)
  - [3.2 Theory](#32-theory)
  - [3.3 Setup](#33-setup)
  - [3.4 Procedures](#34-procedures)
  - [3.5 Data](#35-data)
  - [3.6 Analysis](#36-analysis)
  - [3.7 Results](#37-results)
  - [3.8 Discussion](#38-discussion)
  - [3.9 QA (Short Answers)](#39-qa-short-answers)
- [4. Experiment 02 — Pulse‑Code Modulation (PCM)](#4-experiment-02--pulsecode-modulation-pcm)
  - [4.1 Objective](#41-objective)
  - [4.2 Theory](#42-theory)
  - [4.3 Setup](#43-setup)
  - [4.4 Procedures](#44-procedures)
  - [4.5 Data](#45-data)
  - [4.6 Analysis](#46-analysis)
  - [4.7 Results](#47-results)
  - [4.8 Discussion](#48-discussion)
  - [4.9 QA (Short Answers)](#49-qa-short-answers)
- [5. Data Dictionary (Traceability)](#5-data-dictionary-traceability)
- [6. Reproducibility Checklist](#6-reproducibility-checklist)
- [7. Limitations and Error Sources](#7-limitations-and-error-sources)
- [8. Conclusion](#8-conclusion)
- [9. References](#9-references)

---

## 0. Overview
This report implements and validates **Analog FM** and **Digital PCM** on a modular telecommunications trainer. The design of this README follows a **repeatable lab workflow**:

**Overview → Setup → Procedures → Data → Analysis → Results → Discussion → QA**

**What you’ll find here**
- **FM:** Frequency deviation \( \Delta f \) vs message amplitude \( A_m \), modulation index \( \beta=\Delta f/f_m \), spectrum around \( f_c \)
- **PCM:** Nyquist sampling verification, quantization behavior, **SNR vs bit‑depth**, and (optional) codec loopback/BER

---

## 1. Platform and Safety
**Trainer:** Emona **ETT‑101**  
**Instrumentation:** Digital Storage Oscilloscope (DSO), Function Generator  
**General safety & quality**
- Use **10× probes**; verify probe compensation and scope calibration.
- Avoid rail clipping; keep **headroom** in analog stages.
- Record several readings per point (5–10) and report **mean ± std**.
- Keep cables short, check grounds, and avoid ground loops.

---

## 2. Repository Pointers
If you choose to keep artifacts organized, use this optional structure:
