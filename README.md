# reaper-mastering-toolkit

⚠️ **Work in Progress (Practice-Based Research Toolkit)**  
This repository documents an evolving set of tools developed through applied mastering practice for singles and albums.  
The codebase is **not frozen** and is expected to change as workflows, heuristics, and technical approaches evolve.

---

## Overview

This repository contains a research-oriented toolkit for **music mastering workflows**, implemented primarily within **REAPER** using **Lua scripting**, with optional calls to **Python-based analysis** from Lua.

Mastering is treated here as a constrained and well-defined audio process:  
the processing of a **single stereo signal** with the goal of achieving translation, consistency, and technical compliance across playback contexts.

Rather than focusing on full automation or commercial-grade solutions, this toolkit explores how **procedural decisions in mastering** can be formalized, inspected, and reproduced through code.

---

## Scope and Motivation

The tools in this repository are developed from ongoing professional work as a mastering engineer, addressing recurring tasks such as:

- level normalization and gain staging,
- spectral balance assessment,
- dynamics control heuristics,
- quality-control checks,
- preparation of masters for release formats.

The project is motivated by the question:

> *Which aspects of mastering practice can be expressed as transparent, repeatable procedures, and which must remain perceptual and judgment-based?*

---

## Technical Stack

- **DAW:** REAPER  
- **Primary scripting language:** Lua (ReaScript API)  
- **Analysis layer:** Python (called from Lua when needed)

REAPER is used as the execution environment for audio processing and plugin control, while Python is employed for offline or semi-offline analysis (e.g. feature extraction, statistics, or decision support).

---

## Design Principles

- **Inspectability over automation**  
  All scripts are readable and modifiable; no black-box processing is assumed.

- **Reproducibility over presets**  
  Decisions are encoded procedurally rather than relying solely on fixed plugin presets.

- **Practice-driven developme**
