# reaper-mastering-toolkit

###⚠️ **Work in Progress**
This repository documents an evolving set of tools developed through applied mastering practice for singles and albums.  

---

## Overview

This repository contains a research-oriented toolkit for **music mastering workflows**, implemented primarily within **REAPER** using **Lua scripting**, with optional calls to **Python-based analysis** from Lua.

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

> *Which aspects of mastering practice can be expressed as transparent, repeatable procedures, and which must remain perceptual and judgment-based?*

---

## Requirements

- **DAW:** REAPER
- **Mastering Software:** Izotope Ozone 10
- **Primary scripting language:** Lua (ReaScript API)  
- **Analysis layer:** Python (called from Lua when needed)

---

## Design Principles

- **Reproducibility**  
  Decisions are encoded procedurally rather than relying on plugin presets.

- **Practice-driven developme**
