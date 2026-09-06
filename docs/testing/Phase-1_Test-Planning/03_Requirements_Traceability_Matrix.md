# Requirements Traceability Matrix (RTM)

> Documentation Notice
>
> This Requirements Traceability Matrix was reconstructed after project
> completion using the system workflow, use cases, testing procedures,
> and recorded test cases documented in the thesis manuscript.
>
> It is intended for documentation and archival purposes.

---

# Purpose

The Requirements Traceability Matrix (RTM) establishes traceability between documented system requirements and the corresponding test cases used to evaluate them.

The matrix helps demonstrate that documented functionalities are represented by at least one testing activity.

---

# Requirement Coverage Matrix

| Requirement ID | Functional Requirement | Test Case ID |
|----------------|------------------------|--------------|
| FR-001 | Upload a valid supported video | TC-001 |
| FR-002 | Reject oversized files greater than 500 MB | TC-002 |
| FR-003 | Reject videos exceeding the supported duration limit | TC-002 |
| FR-004 | Reject unsupported file formats | TC-002 |
| FR-005 | Display uploaded video preview | TC-001 |
| FR-006 | Detect object instances from uploaded video | TC-003 |
| FR-007 | Generate instance masks | TC-003 |
| FR-008 | Allow navigation between detected instances | TC-003 |
| FR-009 | Support manual color assignment to object instances | TC-004 |
| FR-010 | Support global style preset selection | TC-005 |
| FR-011 | Generate colorized or recolorized video output | TC-006 |
| FR-012 | Preserve object boundary containment during colorization | TC-007 |
| FR-013 | Preserve object color consistency across frames | TC-008 |
| FR-014 | Allow downloading of generated output video | TC-009 |
| FR-015 | Store completed sessions in history | TC-010 |
| FR-016 | Support multiple object instances with different colors | TC-011 |
| FR-017 | Allow replacement or reset of uploaded videos | TC-012 |
| FR-018 | Support scene or environment preset selection | TC-013 |
| FR-019 | Support style intensity adjustment | TC-014 |

---

# Test Case Reference

## TC-001

**Scenario:** Valid Video Upload

Verifies successful upload and preview of supported video files.

---

## TC-002

**Scenario:** Invalid Video Upload

Verifies validation of:

- Unsupported formats
- Oversized files
- Excessive duration

---

## TC-003

**Scenario:** Object Instance Identification

Verifies:

- Object detection
- Instance mask generation
- Instance navigation

---

## TC-004

**Scenario:** Manual Object Color Assignment

Verifies assignment of user-selected colors to specific detected instances.

---

## TC-005

**Scenario:** Global Style Preset Selection

Verifies registration and application of selected style presets.

---

## TC-006

**Scenario:** Video Generation Process

Verifies successful output generation.

---

## TC-007

**Scenario:** Generated Mask Verification

Verifies object boundary containment.

---

## TC-008

**Scenario:** Temporal Consistency Verification

Verifies object color stability across frames.

---

## TC-009

**Scenario:** View and Download Output

Verifies successful output download.

---

## TC-010

**Scenario:** History Logging

Verifies storage and retrieval of completed processing sessions.

---

## TC-011

**Scenario:** Multiple Instance Color Assignment

Verifies independent color retention across multiple detected instances.

---

## TC-012

**Scenario:** Video Reset or Replace

Verifies clearing and replacement of previous session state.

---

## TC-013

**Scenario:** Scene Environment Preset

Verifies environmental preset selection and processing behavior.

---

## TC-014

**Scenario:** Style Intensity Adjustment

Verifies output differences between varying style intensities.

---

# Coverage Summary

## Functional Requirements

19

## Mapped Requirements

19

## Coverage Rate

100%

---

# Traceability Assessment

All reconstructed functional requirements identified from the documented system workflow are linked to at least one recorded test case.

This matrix provides traceability between:

- System functionality
- Testing activities
- Recorded test evidence

and supports the completeness of the documented testing process.

---

# Conclusion

The documented test cases collectively provide coverage for the primary workflow of the system, including input handling, object processing, style conditioning, video generation, and output management.

This matrix serves as a reference between documented functionality and documented testing evidence.
