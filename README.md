# reaper-mastering-toolkit

#### ⚠️ **Work in Progress**
This repository documents an evolving set of tools developed through applied mastering practice for singles and albums.  

---

## Overview

This repository contains a research-oriented toolkit for **music mastering workflows**, implemented primarily within **REAPER** using **Lua scripting**, with optional calls to **Essentia-based analysis in Python** from Lua.

Mastering is treated here as a constrained and well-defined audio process:  
the processing of a **single stereo signal** with the goal of achieving consistency across various playback contexts.

The toolkit focuses on how **procedural decisions in mastering** can be formalized and reproduced through code.

---

## Scope and Motivation

The tools in this repository are developed from my ongoing professional work as a mastering engineer, addressing recurring tasks such as:

- level normalization and gain staging
- spectral balance assessment
- multiband dynamics control heuristics
- quality-control

The project is motivated by the question:

> *Which aspects of mastering practice can be expressed as repeatable procedures, and which must remain perceptual and judgment-based?*

---

## Tools

- **DAW:** REAPER
- **Mastering Software:** Izotope Ozone 10
- **Primary scripting language:** Lua (ReaScript API)  
- **Analysis layer:** Python + Essentia for measurement (called from Lua)
- **Inspection and validation:** Sonic Visualiser

### Related Work

This project is informed by previous research on spectral similarity analysis, **CSpectra2021**, which explores the comparison of audio signals using spectral descriptors in REAPER-based workflows.
_Reference repository:_
https://github.com/mat2021/CSPECTRA2021

---

## Design Principles

- #### **Reproducibility**  
  Decisions are encoded procedurally rather than relying on plugin presets.

- #### **Practice-driven development**
  Scripts are derived from real mastering sessions and refined through repeated use.

---

## Status

⚠️ Work in Progress

This repository is not a finalized research artifact.  
It reflects an active process of experimentation based on applied mastering work.

Changes include:
- refactoring of scripts
- addition/removal of tools
- changes in Python–Lua interaction
- reorganization of the folder structure

A stable snapshot will be tagged in the near future.

## Audience

This repository is intended for:
- researchers and students interested in **practice-based tool development** for audio production
- musicians interested in procedural approaches to mastering
- reviewers evaluating research portfolios
