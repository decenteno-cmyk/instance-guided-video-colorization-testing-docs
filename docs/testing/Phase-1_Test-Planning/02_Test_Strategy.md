# Test Strategy

> Documentation Notice
>
> This document was reconstructed from the testing methodology,
> evaluation procedures, and results documented in the thesis.
> It is intended for documentation and archival purposes.

---

# Strategy Overview

The testing strategy combines functional testing, internal evaluation, quantitative assessment, and user acceptance evaluation.

The objective of the strategy is to evaluate whether the system performs according to its intended purpose while maintaining acceptable usability, reliability, consistency, and output quality.

---

# Testing Objectives

The testing process aims to verify:

1. Functional correctness of system features.
2. Object-level color assignment accuracy.
3. Temporal consistency across video frames.
4. Boundary containment of applied colors.
5. Global style conditioning effectiveness.
6. System responsiveness and operational stability.
7. User satisfaction and quality in use.

---

# Testing Approaches

## Black Box Testing

### Description

Black Box Testing evaluates the observable behavior of the system without examining source code or internal implementation details.

### Scope

The following features were evaluated:

- Video Upload
- Video Validation
- Video Preview
- Object Detection
- Color Assignment
- Style Selection
- Video Generation
- Output Download
- Session History

### Expected Outcome

Users should be able to complete the intended workflow and obtain a generated output without encountering blocking errors.

---

## White Box Testing

### Description

White Box Testing evaluates internal processes, metric computations, and consistency between system behavior and reported outputs.

### Scope

Evaluation focused on:

- Runtime calculations
- Quantitative evaluation metrics
- Internal processing behavior
- Component contribution analysis

### Expected Outcome

Changes in system components should produce predictable and explainable changes in reported metrics.

---

# Acceptance Testing

## Alpha Testing

### Purpose

Identify major functionality and usability concerns before broader evaluation.

### Focus Areas

- Workflow completeness
- Feature availability
- User interaction flow
- Input validation

---

## Beta Testing

### Purpose

Evaluate the system under realistic usage conditions using representative users.

### Focus Areas

- Effectiveness
- Efficiency
- Satisfaction

### Participants

- Multimedia Arts Students
- Multimedia Arts Faculty
- Industry Professionals

---

# Quantitative Evaluation Strategy

The study uses objective metrics to evaluate output quality and system behavior.

---

## Object-Level Evaluation

### Instance Color Accuracy (ICA)

Measures how accurately object colors are applied within instance boundaries.

### Boundary Leakage Score (BLS)

Measures the degree of undesired color spread outside object boundaries.

---

## Temporal Evaluation

### Flicker Score

Measures frame-to-frame color instability within tracked objects.

### Temporal Color Variance (TCV)

Measures long-term object color stability throughout a video sequence.

---

## Style Evaluation

### Global Palette Coverage (GPC)

Measures how effectively generated backgrounds align with the selected global palette.

---

## Perceptual Evaluation

### Structural Similarity Index (SSIM)

Measures preservation of structural information between frames.

### Learned Perceptual Image Patch Similarity (LPIPS)

Measures perceptual consistency based on deep feature representations.

---

# User Evaluation Strategy

User evaluation follows the ISO/IEC 25019 Quality-in-Use framework.

---

## Effectiveness

Evaluates whether users can successfully achieve intended colorization goals.

Sample areas evaluated:

- Correct color application
- Color consistency
- Boundary preservation
- Style adherence

---

## Efficiency

Evaluates operational performance during system use.

Sample areas evaluated:

- Responsiveness
- Processing time
- Reliability
- Workflow continuity

---

## Satisfaction

Evaluates overall user perception of the system.

Sample areas evaluated:

- Ease of use
- Confidence in outputs
- Interface clarity
- Overall experience

---

# Data Collection Strategy

## Quantitative Data

Collected through:

- Automated metric computation
- Runtime logging
- Performance measurements

## Qualitative Data

Collected through:

- Survey questionnaires
- User feedback
- Interview responses

---

# Success Criteria

The strategy considers the evaluation successful when:

- Functional workflows can be completed successfully.
- Evaluation metrics remain within acceptable thresholds.
- Users provide positive quality-in-use assessments.
- Output quality demonstrates acceptable object-level and temporal consistency.

---

# Testing Deliverables

The testing process produces the following documentation:

- Test Plan
- Test Strategy
- Requirements Traceability Matrix
- Test Cases
- Test Execution Report
- Evaluation Observation Log
- Performance Test Report
- User Acceptance Test Report
- Test Closure Report

---

# Strategy Summary

This testing strategy combines:

- Functional verification
- Internal verification
- Quantitative evaluation
- User-centered evaluation

to provide a structured assessment of the system within the defined scope of the study.
