# Performance Test Report

> Documentation Notice
>
> This document was reconstructed from the quantitative evaluation
> results, operational efficiency measurements, and performance analyses
> reported in the thesis manuscript.
>
> It is intended for documentation and archival purposes.

---

# Report Information

## Document Title

Performance Test Report

## Project

Instance-Guided Semantic Video Colorization Using Diffusion Models

## Version

1.0

---

# Purpose

The purpose of this document is to summarize the quantitative performance evaluation of the system using the Full Proposed Method configuration.

The evaluation focused on:

- Object-level color accuracy
- Boundary containment
- Temporal consistency
- Style conditioning
- Perceptual quality
- Runtime efficiency

---

# Evaluation Metrics

The study used the following quantitative metrics.

---

## Object-Level Metrics

### Instance Color Accuracy (ICA)

Measures object-specific color fidelity inside tracked instance masks.

### Boundary Leakage Score (BLS)

Measures the degree of color leakage outside object boundaries.

---

## Temporal Metrics

### Object-Level Flicker Score

Measures frame-to-frame object color inconsistency.

### Temporal Color Variance (TCV)

Measures long-term color stability throughout a video sequence.

---

## Style Metric

### Global Palette Coverage (GPC)

Measures how effectively output backgrounds conform to the selected style palette.

---

## Perceptual Metrics

### Structural Similarity Index (SSIM)

Measures structural preservation between frames.

### Learned Perceptual Image Patch Similarity (LPIPS)

Measures perceptual similarity using deep feature representations.

---

# Overall Performance Results

## Full Proposed Method

| Metric | Result |
|----------|---------|
| Global Palette Coverage (GPC) | 0.551 |
| Instance Color Accuracy (ICA) | 8.17 ΔE |
| Boundary Leakage Score (BLS) | 3.28 ΔE |
| Flicker Score | 1.09 ΔE/f |
| Temporal Color Variance (TCV) | 1.87 ΔE² |
| SSIM | 0.922 |
| LPIPS | 0.088 |

---

# Interpretation of Results

## Object-Level Accuracy

### ICA = 8.17 ΔE

Interpretation:

- Within the documented healthy range.
- Indicates accurate object-level color assignment.

### BLS = 3.28 ΔE

Interpretation:

- Within the documented healthy range.
- Indicates effective boundary containment.

---

## Temporal Stability

### Flicker = 1.09 ΔE/f

Interpretation:

- Well below the documented threshold.
- Indicates stable object colors between frames.

### TCV = 1.87 ΔE²

Interpretation:

- Within the documented healthy range.
- Indicates strong long-term color stability.

---

## Style Conditioning

### GPC = 0.551

Interpretation:

- Indicates successful global palette conditioning.
- Demonstrates effective scene-level style adherence.

---

## Perceptual Quality

### SSIM = 0.922

Interpretation:

- Strong structural preservation.
- Limited frame-to-frame distortion.

### LPIPS = 0.088

Interpretation:

- High perceptual consistency.
- Low perceptual drift between consecutive frames.

---

# Performance Across Video Categories

## Evaluation Categories

The system was evaluated using three video complexity categories:

1. Simple
2. Moderate
3. Low Light / Noise

---

## Results

| Video Category | GPC | ICA | BLS | Flicker | SSIM | LPIPS | Runtime (s/f) |
|---------------|------|------|------|----------|--------|---------|--------------|
| Simple | 0.571 | 6.91 | 2.74 | 0.87 | 0.968 | 0.067 | 0.0021 |
| Moderate | 0.548 | 8.43 | 3.58 | 1.32 | 0.932 | 0.076 | 0.0034 |
| Low Light / Noise | 0.534 | 9.18 | 4.11 | 1.88 | 0.866 | 0.118 | 0.0028 |

---

# Runtime Analysis

## Runtime Results

| Category | Runtime (s/frame) |
|-----------|-------------------|
| Simple | 0.0021 |
| Moderate | 0.0034 |
| Low Light / Noise | 0.0028 |

### Interpretation

Observed runtime increases correspond to:

- Greater object counts.
- Increased scene complexity.
- Additional processing requirements.

All reported runtimes remained below the study's documented practical threshold.

---

# Operational Stability

## Failure Count

| Category | Failures |
|-----------|-----------|
| Simple | 0 |
| Moderate | 0 |
| Low Light / Noise | 0 |

### Interpretation

No tracking fallback events or operational failures were recorded during documented evaluation runs.

---

# Computational Complexity Summary

The study identified diffusion denoising as the dominant computational cost.

### Primary Time Complexity

```text
O(τ × L × h × w × d²)
```

Where:

- τ = Diffusion steps
- L = U-Net layers
- h × w = Latent resolution
- d = Feature depth

### Additional Costs

- Instance mask gating
- Identity propagation
- Palette evaluation

These operations scale linearly relative to instance count.

---

# Key Findings

The quantitative evaluation indicates:

1. Strong object-level color accuracy.
2. Effective boundary containment.
3. High temporal stability.
4. Successful style conditioning.
5. Consistent perceptual quality.
6. Stable runtime performance.
7. Zero documented operational failures.

---

# Conclusion

The documented evaluation results indicate that the Full Proposed Method maintained acceptable performance across all evaluated categories.

The system demonstrated object-level color control, temporal consistency, style adherence, and operational stability while remaining within the performance thresholds defined by the study.
