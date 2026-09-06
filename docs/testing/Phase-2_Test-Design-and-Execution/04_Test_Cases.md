# Test Cases

> Documentation Notice
>
> This document was reconstructed from the recorded test cases
> documented in Appendix I of the thesis manuscript.
>
> It is intended for documentation and archival purposes.

---

# Overview

This document contains the functional test cases used to evaluate the system workflow.

The test cases focus on:

- Input validation
- Object detection
- Color assignment
- Style configuration
- Video generation
- Output management
- Temporal consistency

---

# TC-001: Valid Video Upload and Preview

## Objective

Verify that the system accepts a valid video file and displays a preview.

## Preconditions

- Application is launched.

## Test Steps

1. Launch the application.
2. Click the **Start Creating** button.
3. Select a valid video file.

## Expected Result

- The system accepts the file.
- The video uploads successfully.
- A preview is displayed.

## Recorded Result

As Expected

## Status

PASS

---

# TC-002: Invalid Video Upload

## Objective

Verify that the system correctly rejects invalid video files.

## Preconditions

- Application is launched.

## Test Steps

### Scenario A

1. Upload a file larger than 500 MB.

### Expected Result

The system rejects the file and displays a file size warning.

---

### Scenario B

1. Upload a video longer than 15 seconds.

### Expected Result

The system rejects the file and displays a duration warning.

---

### Scenario C

1. Upload an unsupported file format.

### Expected Result

The system rejects the file and displays a supported format message.

## Recorded Result

As Expected

## Status

PASS

---

# TC-003: Object Instance Identification

## Objective

Verify object detection and instance generation.

## Preconditions

- Valid video uploaded.

## Test Steps

1. Proceed to object detection.
2. Wait for processing.
3. Navigate through identified objects.

## Expected Result

- Object instances are detected.
- Instance masks are displayed.
- Navigation between instances functions correctly.

## Recorded Result

As Expected

## Status

PASS

---

# TC-004: Manual Object Color Assignment

## Objective

Verify assignment of colors to selected object instances.

## Preconditions

- Object instances detected.

## Test Steps

1. Select an object instance.
2. Choose a color.
3. Apply the selected color.

## Expected Result

- Selected instance receives assigned color.
- User interface reflects the assignment.

## Recorded Result

As Expected

## Status

PASS

---

# TC-005: Global Style Preset Selection

## Objective

Verify style preset selection.

## Preconditions

- Color assignment step completed.

## Test Steps

1. Open the style configuration module.
2. Select a style preset.

## Expected Result

- Style selection is registered.
- Selected preset is applied during processing.

## Recorded Result

As Expected

## Status

PASS

---

# TC-006: Video Generation Process

## Objective

Verify generation of the final output video.

## Preconditions

- Video uploaded.
- Color assignments completed.
- Style selected.

## Test Steps

1. Click Generate.
2. Wait for processing to complete.

## Expected Result

- Generation completes successfully.
- Final video output is displayed.

## Recorded Result

As Expected

## Status

PASS

---

# TC-007: Generated Mask Verification

## Objective

Verify color containment within object boundaries.

## Preconditions

- Output video generated.

## Test Steps

1. Play generated output.
2. Inspect object boundaries.

## Expected Result

- Assigned colors remain within intended mask regions.
- Minimal or no visible boundary leakage.

## Recorded Result

As Expected

## Status

PASS

---

# TC-008: Temporal Consistency Verification

## Objective

Verify object color stability across video frames.

## Preconditions

- Output video generated.

## Test Steps

1. Play generated video.
2. Observe target objects during motion.

## Expected Result

- Objects retain consistent color identity.
- Severe flickering is not observed.

## Recorded Result

As Expected

## Status

PASS

---

# TC-009: View and Download Output

## Objective

Verify output downloading functionality.

## Preconditions

- Video generation completed.

## Test Steps

1. Click Download.

## Expected Result

- Output video is successfully saved to local storage.

## Recorded Result

As Expected

## Status

PASS

---

# TC-010: Session History

## Objective

Verify storage of completed processing sessions.

## Preconditions

- At least one completed generation session exists.

## Test Steps

1. Complete a generation session.
2. Open the History section.

## Expected Result

- Completed session appears in history.
- Entry can be viewed and accessed.

## Recorded Result

As Expected

## Status

PASS

---

# TC-011: Multiple Instance Color Assignment

## Objective

Verify support for multiple independently colored instances.

## Preconditions

- Multiple object instances detected.

## Test Steps

1. Assign distinct colors to multiple instances.
2. Generate output.

## Expected Result

- Each object retains its assigned color.
- Colors do not bleed across instances.

## Recorded Result

As Expected

## Status

PASS

---

# TC-012: Video Reset or Replace

## Objective

Verify replacement of previously uploaded videos.

## Preconditions

- Existing session in progress.

## Test Steps

1. Return to upload stage.
2. Upload a different video.

## Expected Result

- Previous session state is cleared.
- New processing cycle begins.

## Recorded Result

As Expected

## Status

PASS

---

# TC-013: Scene Environment Preset

## Objective

Verify scene preset processing.

## Preconditions

- Video uploaded.

## Test Steps

1. Process the same video using different presets.

## Expected Result

- Preset selection influences system processing behavior.

## Recorded Result

As Expected

## Status

PASS

---

# TC-014: Style Intensity Adjustment

## Objective

Verify the effect of style intensity settings.

## Preconditions

- Style selection available.

## Test Steps

1. Process identical video using the same style.
2. Apply different intensity levels.

## Expected Result

- Higher intensity produces a stronger stylistic effect.
- Lower intensity produces a weaker stylistic effect.

## Recorded Result

As Expected

## Status

PASS

---

# Summary

## Total Test Cases

14

## Recorded Passes

14

## Recorded Failures

0

## Coverage Areas

- Video Upload
- Input Validation
- Object Detection
- Color Assignment
- Style Configuration
- Video Generation
- Boundary Verification
- Temporal Consistency
- Output Management
- Session Management

These test cases collectively cover the primary workflow documented for the system.
