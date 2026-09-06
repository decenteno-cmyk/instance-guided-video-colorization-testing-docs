# Instance-Guided Video Colorization Testing Documentation

## Documentation Notice

This repository contains reconstructed software testing documentation derived from the completed thesis manuscript:

**Instance-Guided Semantic Video Colorization Using Diffusion Models**. The documents were created after project completion using the testing methodology, evaluation procedures, quantitative results, and recorded test cases reported in the study. This repository is intended for documentation, archival, and academic reference purposes. Source code is not included.

---

# Repository Purpose

The objective of this repository is to organize the testing and evaluation evidence reported in the thesis into standard software testing artifacts.

The repository does **not** claim that these documents existed during development. Instead, they serve as a structured reconstruction of the documented testing activities and results reported in the final manuscript. 

---

# Project Overview

The study developed an instance-guided semantic video colorization framework that combines diffusion-based video generation with object-level conditioning, identity propagation, structural constraints, and style conditioning. The system supports both grayscale video colorization and selective object recolorization while maintaining temporal consistency across frames. 

The architecture incorporates:

- Grounding DINO for object detection. 
- SAM 2 for instance segmentation. 
- CoTracker for identity propagation. 
- XMem for mask propagation. 
- ControlNet for structural conditioning. 
- Stable Diffusion–based video generation. 
- LoRA-based style conditioning. 

---

# Repository Structure

```text
docs/
└── testing/
    │
    ├── Phase-1_Test-Planning/
    │   ├── 01_Test_Plan.md
    │   ├── 02_Test_Strategy.md
    │   └── 03_Requirements_Traceability_Matrix.md
    │
    ├── Phase-2_Test-Design-and-Execution/
    │   ├── 04_Test_Cases.md
    │   ├── 05_Test_Execution_Report.md
    │   └── 06_Evaluation_Observation_Log.md
    │
    └── Phase-3_Test-Evaluation-and-Closure/
        ├── 07_Performance_Test_Report.md
        ├── 08_User_Acceptance_Test_Report.md
        └── 09_Test_Closure_Report.md
```

---

# Documentation Phases

## Phase 1 – Test Planning

This phase defines what was intended to be tested, how testing would be conducted, and how system functionality relates to recorded test activities.

### Included Documents

| Document | Purpose |
|-----------|----------|
| Test Plan | Defines testing scope, objectives, and environment |
| Test Strategy | Describes testing methodologies and evaluation approaches |
| Requirements Traceability Matrix | Maps requirements to documented test cases |

---

## Phase 2 – Test Design and Execution

This phase documents the test cases reported in the thesis and summarizes the recorded execution outcomes.

### Included Documents

| Document | Purpose |
|-----------|----------|
| Test Cases | Functional test case documentation |
| Test Execution Report | Summary of recorded execution results |
| Evaluation Observation Log | Observed performance changes derived from evaluation results and ablation analyses |

---

## Phase 3 – Test Evaluation and Closure

This phase documents the final evaluation outcomes and testing conclusions.

### Included Documents

| Document | Purpose |
|-----------|----------|
| Performance Test Report | Quantitative system evaluation |
| User Acceptance Test Report | ISO/IEC 25019 Quality-in-Use results |
| Test Closure Report | Final testing summary and conclusions |

---

# Testing Approaches

The thesis utilized multiple approaches to evaluate the system. 

## Black Box Testing

Evaluated externally observable behavior including:

- Video upload
- Input validation
- Object detection
- Color assignment
- Style selection
- Video generation
- Export functionality

## White Box Testing

Evaluated:

- Internal metric calculations
- Implementation behavior
- Consistency between observed outputs and computed evaluation metrics

## User Evaluation

The study evaluated user perception using ISO/IEC 25019 Quality-in-Use criteria. 

Assessment areas included:

- Effectiveness
- Efficiency
- Satisfaction
---

# Documented Test Coverage

The thesis appendix reports fourteen test scenarios covering the primary system workflow.

These scenarios include:

- Video Upload
- Invalid Input Handling
- Object Detection
- Manual Color Assignment
- Style Preset Selection
- Video Generation
- Boundary Verification
- Temporal Consistency Verification
- Video Download
- Session History
- Multi-Instance Color Assignment
- Session Reset
- Scene Presets
- Style Intensity Adjustment

---

# Evaluation Overview

The study evaluated system behavior through custom quantitative metrics designed to measure object-level accuracy, temporal stability, style conditioning, and perceptual quality.

Primary metrics include:

- Global Palette Coverage (GPC)
- Instance Color Accuracy (ICA)
- Boundary Leakage Score (BLS)
- Flicker Score
- Temporal Color Variance (TCV)
- Structural Similarity Index (SSIM)
- Learned Perceptual Image Patch Similarity (LPIPS)

---

# User Evaluation Overview

The system was evaluated by a purposively selected group of respondents consisting of:

- 35 FEU Tech Multimedia Arts Students
- 5 FEU Tech Multimedia Arts Faculty Members
- 10 Creative Industry and Cultural Preservation Professionals

Total Respondents: **50**. 

---

# Limitations

This repository should be interpreted as a documentation repository rather than a software repository.

Specifically:

- Source code is not included.
- Development artifacts are not included.
- Version control history from the original project is not included.
- The testing documents are reconstructed from the final thesis manuscript and supporting records.

---

# Intended Use

This repository may be used as:

- An archive of testing documentation.
- A reference for software testing documentation structure.
- A companion repository for the thesis manuscript.
- An example of reconstructed QA documentation based on completed academic research.

---

# Authors

**Bachelor of Science in Computer Science**  
**Specialization in Software Engineering**  
**FEU Institute of Technology**

- Centeno, Deanne Yzabelle E. (QA)
- Delos Santos, Marie Ysabel B. (Documentation)
- Mangahas, Karl Stephen D. (Project Manager)
- Plaus, Tristan J. (Developer)
2026 
