# COIMATRON
**Plates Recognition AI**

---

## General Description
This project consists of a series of models executed simultaneously using **YOLOv8**. The models activate when a plate enters the bottom right of the screen.

---

## Cars and Plates Model
The first model detects both cars and plates using the variable `Model_Plates`.

---

## Tracking
The tracking component activates after a plate is detected by the first model. This part assigns an ID to the plate and tracks it. If a plate is being tracked, the first model will not detect that plate again.

---

## Screenshot
Once a plate is being tracked, the next component executes. It takes a screenshot of the plate and displays it in the top right corner of the screen to show the original plate.

---

## Numbers Model
The final part activates once the screenshot is taken. It reads the numbers and letters from the plate in the screenshot from left to right and displays them alongside the ID on the tracking bounding box.

---

## Git Repositories and Required Libraries
- **Git Repository**:
  -Sort
- **Libraries**:
  - Ultralytics
  - OpenCV
  - Numpy

---

## Installation
To install the required libraries, run the following command:

```bash
pip install ultralytics opencv-python numpy
