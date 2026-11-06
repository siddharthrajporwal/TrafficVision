# TrafficVision 🚦

### AI-Based Real-Time Traffic Violation Detection and Automatic Number Plate Recognition System

**An AI-powered traffic monitoring prototype using Computer Vision, Deep Learning and Optical Character Recognition.**

---

## 1. Project Overview

TrafficVision is an AI-based system designed to detect selected traffic violations from traffic video footage and identify vehicle registration numbers using Automatic Number Plate Recognition (ANPR).

The system aims to integrate object detection, image processing and Optical Character Recognition (OCR) to identify suspected violations, extract vehicle number plates, and maintain timestamped violation records.

It will also include a local database for vehicle information and a warning-generation mechanism for demonstration purposes.

## 2. Project Objectives

- Process live or pre-recorded traffic video footage.
- Detect vehicles and riders using computer vision.
- Identify selected traffic violations, initially focusing on helmet-related violations.
- Detect and extract vehicle number plates.
- Recognise registration numbers using OCR.
- Maintain vehicle and violation records in a local database.
- Generate warning notifications for identified test records.
- Provide a visual monitoring interface through a planned frontend dashboard.

## 3. Proposed System Architecture

The proposed system follows this workflow:

1. **Video Input:** Capture traffic footage through a camera or pre-recorded video.
2. **Frame Processing:** Extract and preprocess individual video frames using OpenCV.
3. **Object Detection:** Detect vehicles, riders and relevant objects.
4. **Violation Detection:** Identify suspected traffic violations.
5. **Number Plate Detection:** Locate and extract vehicle registration plates.
6. **OCR Processing:** Recognise registration numbers from extracted plate images.
7. **Database Lookup:** Match recognised registration numbers against locally stored test vehicle records.
8. **Violation Logging:** Store violation details, timestamps and associated evidence.
9. **Warning Generation:** Generate prototype warnings for identified records.
10. **Visualisation:** Display monitoring information and violation records through the planned frontend.

## 4. Technology Stack

| Component | Proposed Technology |
|---|---|
| Programming Language | Python |
| Video Processing | OpenCV |
| Object Detection | YOLO |
| Number Plate Recognition | Computer Vision + OCR |
| OCR Engine | EasyOCR / Tesseract |
| Database | SQLite |
| Backend API | FastAPI (planned) |
| Frontend | React (planned) |

*The final technology choices may be refined during development.*

## 5. Repository Structure

```text
TrafficVision/
│
├── README.md
├── .gitignore
│
├── src/
│   ├── detection/
│   ├── number_plate/
│   └── ocr/
│
├── models/
├── data/
├── docs/
│   └── Group8_ProjectPlan.docx
│
└── tests/
```

### Directory Description

- **src/** – Main Python source code.
  - `detection/` – Vehicle, rider and violation detection.
  - `number_plate/` – Number plate detection and extraction.
  - `ocr/` – Registration number recognition.
- **models/** – Pretrained or fine-tuned AI models.
- **data/** – Sample traffic footage and testing data.
- **docs/** – Project proposals, architecture diagrams and technical documentation.
- **tests/** – Testing scripts and evaluation procedures.

A frontend and backend directory structure may be added as development progresses.

## 6. Development Approach

The project will be developed in stages:

- **Phase 1:** Project setup, research and architecture design.
- **Phase 2:** Video processing and object detection.
- **Phase 3:** Traffic violation detection.
- **Phase 4:** Number plate detection and OCR integration.
- **Phase 5:** Database integration and warning generation.
- **Phase 6:** Frontend dashboard development and system integration.
- **Phase 7:** Testing, evaluation and final demonstration.

## 7. Evaluation Criteria

The proposed system will be evaluated using:

- Vehicle and rider detection accuracy.
- Traffic violation detection precision and recall.
- Number plate detection performance.
- OCR recognition accuracy.
- Real-time processing speed (FPS).
- Database logging reliability.
- Overall system performance under different lighting and traffic conditions.

## 8. Team Members

| Name | Student ID |
|---|---|
| Gyaneshwar Karki | 60428 |
| Jayesh Phondani | 60624 |
| Siddharth Raj Porwal | 60459 |
| Suryansh Prakash | 60462 |

**Project Guide:** Dr. P.K. Mishra  
**Associated Teaching Personnel:** Mr. Dheeraj Pandey

**Primary Domain:** Artificial Intelligence & Computer Vision

## 9. Current Development Status

**Current Stage:** Initial Project Planning and Repository Setup.

The project repository and preliminary directory structure have been established. Implementation, model integration, frontend development and testing are planned for subsequent development phases.

## 10. Scope and Limitations

TrafficVision is an academic prototype intended for demonstration and evaluation.

- The initial implementation will focus on a selected traffic violation rather than multiple violation categories.
- Vehicle information will be maintained using a local test database.
- Actual government vehicle registry integration is outside the initial project scope.
- Generated warnings are prototype notifications, not official traffic challans or legal determinations.
- Detection results may require human verification.

## 11. Future Scope

Potential future improvements include:

- Support for additional traffic violations.
- Improved number plate recognition under challenging conditions.
- A web-based traffic monitoring dashboard.
- Real-time notification integration.
- Performance optimisation for larger video streams.
- Integration with external vehicle databases, subject to authorised access.

---

*TrafficVision – Towards Smarter and More Efficient Traffic Monitoring.*
