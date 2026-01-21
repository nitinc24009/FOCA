# FOCA: Multimodal Malware Classification via Hyperbolic Cross-Attention

Official PyTorch implementation of the ICASSP 2026 paper:

**FOCA: Multimodal Malware Classification via Hyperbolic Cross-Attention**  

Authors: Nitin Choudhury*, Bikrant Bikram Pratap Maurya*, Orchid Chetia Phukan, Arun Balaji Buduru

**Accepted at IEEE ICASSP 2026**

(* equal contribution)

---

## Overview

This repository contains the reference implementation of **FOCA**, a multimodal malware classification framework that fuses **audio and visual representations of binaries in hyperbolic space** using a novel **Hyperbolic Cross-Attention (HCA)** mechanism.

The key idea is to explicitly model the **hierarchical relationship between modalities**:
- **Audio representations** capture fine-grained byte-level characteristics
- **Visual representations** capture higher-level structural patterns

FOCA projects both modalities into the **Poincaré ball**, aligns them using curvature-aware cross-attention, and fuses them via Möbius addition.

This code reproduces all experiments reported in the ICASSP 2026 paper.

---

## Contributions Implemented

- Binary-to-audio and binary-to-image transformations
- Multimodal fusion in hyperbolic space
- Hyperbolic Cross-Attention (HCA)
- Comparison against unimodal, Euclidean fusion, and SOTA baselines
- Evaluation on **Mal-Net** and **CICMalDroid2020**

---

## Paper & Citation

If you use this code, please cite:

```bibtex
@inproceedings{choudhury2026foca,
  title     = {FOCA: Multimodal Malware Classification via Hyperbolic Cross-Attention},
  author    = {Choudhury, Nitin and Maurya, Bikrant Bikram Pratap and Phukan, Orchid Chetia and Buduru, Arun Balaji},
  booktitle = {Proceedings of the IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},
  year      = {2026}
}
