# Software-Based-ISP-Pipeline-Implementation
Camera image sensor output(Bayer Pattern)is processed through a software-implemented ISP pipeline to generate a visually correct RGB image.

## Overview
This project implements a simplified Image Signal Processing(ISP) Pipeline in software.
Starting from Bayer-Pattern image data(similar to camera sensor output), the pipeline processes the image step-by-step to generate a visually correct RGB image.

The goal of this project is to understand how raw sensor data is transformed into a final image inside camera systems and vision-based embedded systems.

## Motivation 
In camera-based systems such as robotics and embedded vision, image quality and processing latency are critical.
Before high-level vision algorithms can be applied, raw sensor data must be processed through an ISP.

This project focuses on understanding the fundamental ISP blocks by implementing them in software. 

## ISP Pipeline Structure
The implemented ISP pipeline consists of the following stages:
1. **Demosaicing**
   - Reconstructs full RGB pixels from Bayer-pattern sensor data
2. **White Balance**
   - Adjusts color channel gains to compensate for illumination conditions
3. **Color Correction**
   - Applies a color correction matrix to account for sensor characteristics
4. **Gamma Correction**
   - Applies nonlinear intensity mapping for perceptual brightness

Each stage is implemented as an independent module and combined as a pipeline.

## Input and Output
- **Input**
  - Bayer-pattern image (Simulated or Extracted from raw sensor data)

- **Output**
  - RGB image after ISP processing


 ## Implementation Details
 - Language: Python
 - Libraries:
   - OpenCV
   - Numpy
- Pipeline Design:
  - Modular Structure
  - Configurable processing parameters
 
## Results
Sample results include:
- Intermediate images after each ISP stage
- Final RGB output images

## Limitations and Future Work
- Simplified demosaicing algorithm
- No hardware acceleration
- Future Extensions:
  - Edge-aware demosaicing
  - Performance Optimization
  - Hardware-oriented pipeline analysis
 
## Author
- Major: Software Convergence
- Interest: Embedded Vision
