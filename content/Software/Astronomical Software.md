---
title: Astronomical Software
tags: software, interferometry
---

Accompanying several written publications, I (or my collaborators) have published software packages in the spirit of open science and for the community to use.

# MATISSE LM Data Reduction
[https://github.com/jwisbell/matisse_lm_datareduction](https://github.com/jwisbell/matisse_lm_datareduction)

Python scripts to process MATISSE LM-band for faint sources.

## Usage
1. First run the standard ESO Data Reduction Software (DRS) pipeline (https://www.eso.org/sci/software/pipelines/) on your target and calibrator
2. Make a config file (see the example in ./scripts) for each observing block (OB)
3. Run the `lm_cflux_cphase_extraction.py` script for each config file.
4. Calibrate the fluxes of your data using the `lm_custompipe_calibration.py` script

From there you have flux calibrated data for each exposure. You can do further Beam Commuting Device (BCD) calibration or averaging of exposures on a single baseline in the standard way for MATISSE. 

This package was used in [The dusty heart of Circnus. II](../Publications/the-dusty-heart-circinus-ii.md) and in my PhD thesis. 

# Gravity Sandbox (Gravbox)
[https://github.com/jwisbell/gravity_sandbox](https://github.com/jwisbell/gravity_sandbox)

Augmented Reality Gravitational Dynamics Sandbox - GravBox - Version 1.0 (December 2017)

Created at the University of Iowa

- Written by Jacob Isbell, Sophie Deam, Jianbo Lu, and Tyler Stercula

- Graphics made by Jeremy Swanson and Jacob Isbell

- Hardware by Mason Reed, Ross McCurty, Sadie Moore, and Wyatt Bettis

- Supervised by Hai Fu

# All-Sky Camera Visualization

[https://github.com/jwisbell/allsky_camera](https://github.com/jwisbell/allsky_camera)

Basic python package for overplotting constellations on an all-sky camera image, for making basic measurements, and for making nightly videos. Briefly used at the University of Iowa before a lightning strike. 

# Faraday Rotation CNN

[https://github.com/jwisbell/faraday_cnn](https://github.com/jwisbell/faraday_cnn)

Scripts accompanying [Brown et al. (2019)](https://ui.adsabs.harvard.edu/abs/2019MNRAS.483..964B/abstract) using convolutional neural networks to estimate Faraday rotation in Square Kilometer Array observations.