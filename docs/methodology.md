# Methodology

## Representation

Each individual is an image generated from layered semi-transparent polygons. Polygons are parameterized by their vertex coordinates and RGBA colors.

## Evolutionary Process

The implementation follows a standard Genetic Algorithm structure:

1. Population initialization.
2. Fitness evaluation.
3. Selection.
4. Crossover.
5. Mutation.
6. Iterative replacement across generations.

## Crossover

The project includes image-space crossover operators:

- Alpha blending between two parent images.
- Mask-based pixel crossover using a binary mask.

## Mutation

Mutation introduces visual variation through:

- structural changes such as adding a polygon,
- pixel-level perturbations in RGBA values.

## Fitness

The optimization fitness is based on average CIE76 ΔE* color difference in Lab color space:

```text
F(candidate) = mean(ΔE*(target, candidate))
```

Lower values indicate a closer perceptual color match.

## Evaluation

Additional metrics are computed for analysis:

- MSE,
- PSNR,
- SSIM,
- LPIPS,
- FID,
- histogram distance,
- perceptual difference heatmaps.
