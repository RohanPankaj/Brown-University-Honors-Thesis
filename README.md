# Characterization of Probabilistic Polarization in Ferroelectric PZT Thin Films

**Rohan S. Pankaj**
Undergraduate Honors Thesis, Brown University School of Engineering
Submitted April 2026, in partial fulfillment of the Sc.B. in Electrical Engineering

- Advisor: Dr. Lucas Caretta, Assistant Professor of Engineering, Brown University
- Reader: Dr. Alexander Zaslavsky, Professor of Engineering and Physics, Brown University
- Honors Committee Chair: Dr. Monica Martinez Wilhelmus, Assistant Professor of Engineering, Brown University

## Abstract

Materials based approaches to True Random Number Generation (TRNG) are an active area of research with a wide range of applications in modeling, simulation, and cybersecurity. This thesis presents the detailed theory and design of a ferroelectric capacitor (FeCAP) which utilizes inherent stochasticity in ferroelectric switching dynamics to create a Physically Unclonable Function (PUF). This is done by using an oxygen-deficient YBCO layer as the top electrode in the capacitor. In doing so, we aim to engineer oxygen vacancies at the PZT/YBCO interface to act as pinning sites for the propagation of polarization switching. This would result in a Barkhausen-like effect wherein stochastic current spikes can be measured and form the basis of a probability distribution. We present data showing cycle-to-cycle variation in switching dynamics well above circuit noise. These measurements resemble the intended Barkhausen-like behavior. This variation was ultimately attributed to incomplete electrical contact between measurement probes and the rough YBCO layer. Still, the wide distribution created by changes in switching dynamics signal that the proposed approach remains an enticing avenue for TRNG.

## Overview

The thesis investigates a ferroelectric capacitor (FeCAP) with a SRO/PZT/YBCO material stack, grown by Pulsed Laser Deposition, as a candidate physically unclonable function (PUF) for true random number generation. Rather than reading the end polarization state after a switching pulse (the standard approach in prior ferroelectric TRNG literature), this work extracts stochasticity directly from the switching *dynamics* :PUND (Positive-Up-Negative-Down) current traces.

Key results:
- Hysteresis and PUND measurements on SRO/PZT/YBCO devices show cycle-to-cycle current variation resembling Barkhausen pulses, in contrast to smooth, repeatable switching in SRO/PZT/Pt control devices.
- P* (switching-isolated polarization) distributions for SRO/PZT/YBCO-1 are bimodal and far wider than circuit noise, suggesting a usable entropy source.
- Follow-up material characterization (AFM, XRD) and a platinum-electrode control device (SRO/PZT/YBCO/Pt-3) show that the observed stochasticity most likely originates from probe-tip contact instability on the rough YBCO surface, rather than the intended oxygen-vacancy pinning of domain walls.
- The thesis concludes that switching-dynamics-based ferroelectric TRNG remains promising, contingent on higher-quality epitaxial YBCO growth and platinum-standard electrodes in future work.

Chapter breakdown: Introduction (motivation, ferroelectric background, LGD theory) → Literature Review (stochastic switching, prior ferroelectric TRNG approaches) → Methodology (sample growth, hysteresis/PUND measurement setup, AFM/PFM, XRD) → Results (control vs. stochastic devices, P* distributions, materials validation) → Discussion and Conclusion.

## Repository Contents

- [`Rohan Pankaj Undergraduate Honors Thesis Signed.pdf`](./Rohan%20Pankaj%20Undergraduate%20Honors%20Thesis%20Signed.pdf) — the full signed thesis.
- Raw measurement data for all thesis figures (hysteresis/PUND traces, AFM, XRD, LGD simulation output) is archived on Zenodo rather than stored in this repo: **[10.5281/zenodo.21109514](https://doi.org/10.5281/zenodo.21109514)**.

### Data included on Zenodo

| Figure | Description |
|---|---|
| 9 | Breakdown of PUND measurements |
| 14 | LGD simulation of the material stack |
| 15 & 16 | Control hysteresis/PUND on SRO/PZT/Pt |
| 17 | Stochastic hysteresis examples across growths and device size |
| 18 | Example hysteresis loops for a 10x10 μm² device on SRO/PZT/YBCO-2 |
| 19 | Stochastic PUND examples across growths and device size |
| 20 | P* vs. cycle for SRO/PZT/YBCO-1 and SRO/PZT/YBCO-2 |
| 21 & 22 | Distribution of P* values, and per-amplitude PUND breakdown, for SRO/PZT/YBCO-1 |
| 23–25 | AFM of unpatterned/patterned SRO/PZT/YBCO-3 and SRO/PZT/YBCO/Pt-3 |
| 26 | Charge transport data on SRO/PZT/YBCO/Pt-3 |
| 27 | XRD of SRO/PZT/YBCO-3 with labeled peaks |

## Software

Measurements were automated and analyzed using [PIEC (Python Integrated Experimental Control)](https://github.com/ElPsyKurisu/piec). Material stack simulations (Figure 14) used the accompanying open-source [FeSim](https://github.com/RohanPankaj/FeSim) software.

## Citation

See [`CITATION.cff`](./CITATION.cff) for machine-readable citation metadata (GitHub renders a "Cite this repository" button from this file).

Pankaj, R. S. (2026). *Characterization of Probabilistic Polarization in Ferroelectric PZT Thin Films.* Undergraduate Honors Thesis, Brown University School of Engineering.

Data: Pankaj, R. S. (2026). Data for "Characterization of Probabilistic Polarization in Ferroelectric PZT Thin Films" [Data set]. Zenodo. https://doi.org/10.5281/zenodo.21109514
