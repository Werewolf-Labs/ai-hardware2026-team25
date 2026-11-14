# University of Virginia
## Department of Electrical and Computer Engineering

**Course:** ECE 4332 / ECE 6332 — AI Hardware Design and Implementation  
**Semester:** Fall 2025  
**Proposal Deadline:** November 5, 2025 — 11:59 PM  
**Submission:** Upload to Canvas (PDF) and to GitHub (`/docs` folder)

--

## 1. Project Title: Face Detection
Name of the Team: Project 25 

Sherina Williams and Brody Ruday

## 2. Platform Selection 
For this project, our team decided to use the OpenMV Cam H7 Plus, a TinyML development board designed for embedded computer vision applications. We chose this platform because we have previous experience working with TinyML hardware and because the OpenMV Cam H7 Plus already includes a camera and a microcontroller

## 3. Problem Definition
Our team aims to implement a simple face recognition system using the OpenMV Cam H7 Plus. The camera will capture images and use an embedded machine learning model to detect and recognize faces directly on the device. The main challenge is running computer vision and AI algorithms on hardware with limited processing power, memory, and energy compared to a traditional computer.

This project is relevant to AI hardware because the face recognition system needs to process images with low latency while using limited computational resources. Performing the AI processing directly on the OpenMV Cam reduces the need to send images to an external computer or cloud server, which can improve response time and reduce communication requirements. 
## 4. Technical Objectives
Detect faces with at least 90 percent recall  under controlled lighting conditions and distance.
Correctly identify registered individuals with at least 85% corrective on the test dataset.
complete face detection and recognition within 3 seconds per frame.

## 5. Methodology
Our team will use the OpenMV Cam H7 Plus as the primary hardware platform. The board already contains the camera and the processing hardware required for the project, so no additional camera or external processing hardware should be necessary for the basic implementation.

The project will begin by setting up the OpenMV development environment and testing the camera using basic image-processing functions. We will then collect or create a small dataset containing images of the individuals that will be registered in the system. Images will be collected under controlled lighting and distance conditions to make the initial testing more consistent.

For the software implementation, we will use MicroPython and the OpenMV libraries to capture images, process the images, detect faces, and perform recognition. We will investigate the machine-learning and computer-vision functionality supported by the OpenMV Cam H7 Plus and select a model or recognition method that can run within the device's memory and processing limitations.

The system will first identify whether a face is present in the camera image. If a face is detected, the system will then compare the detected face with the registered individuals. The output will indicate the identity of the recognized person or identify the face as unknown if it does not meet the required recognition threshold.

The final validation will compare the measured results against the technical objectives established in Section 4. If the initial model does not meet the requirements, we will investigate adjustments such as reducing image resolution, changing model parameters, simplifying the recognition process, or modifying the dataset.
## 6. Expected Deliverables
A working face detection and recognition demonstration running on the OpenMV Cam H7 Plus.
A GitHub repository containing the source code, documentation, and project files.
Documentation describing testing procedure.
A dataset or description of the dataset used for testing and evaluation, where appropriate.
Performance results including recognition accuracy, detection recall, and inference time.
Presentation slides describing the project design, implementation, and results.
A final project report documenting the design process, implementation, testing, and conclusions.
A final demonstration showing the system detecting and recognizing registered faces on the embedded hardware.

## 7. Team Responsibilities

| Name | Role | Responsibilities |
|------|------|------------------|
| [Sherina] | Team Lead | Coordination, documentation |
| [Sherina] | Hardware | Setup, integration |
| [Brody and Sherina] | Software | Model training, inference |
| [Sherina and Brody] | Evaluation | Testing, benchmarking |

## 8. Timeline and Milestones

| Week | Milestone | Deliverable |
|------|------------|-------------|
| 2 | Proposal | PDF + GitHub submission |
| 4 | Midterm presentation | Slides, preliminary results |
| 6 | Integration & testing | Working prototype |
| Dec. 18 | Final presentation | Report, demo, GitHub archive |
