# Project Summary

This project implements a Genetic Algorithm that evolves target images using a population of polygon-based candidate images. Each candidate is rendered as a stack of semi-transparent polygons with variable geometry, color and alpha values.

The optimization objective is to minimize the perceptual color difference between a generated image and a target image using CIE76 ΔE* in Lab color space. Additional metrics such as MSE, PSNR, SSIM, LPIPS, FID and histogram distance are computed for post-hoc analysis and interpretation.

The project was originally developed as a Bio-inspired Learning coursework assignment. The public repository focuses on code organization, documentation, methodological clarity and responsible handling of external visual assets.
