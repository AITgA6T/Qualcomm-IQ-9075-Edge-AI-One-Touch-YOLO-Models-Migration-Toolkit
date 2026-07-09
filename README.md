# Qualcomm IQ-9075 Edge AI One-Touch YOLO Models Migration Toolkit

## Advantages of IQ-9075

1. IQ-9075 can provide up to 200 sparse TOPS of AI computing power and supports GPU and DSP accelerated computing
2. The Qualcomm Neural Processing (SNPE) SDK and the Qualcomm AI Engine Direct (QNN) can optimize the performance of trained neural networks
3. It supports Yocto and Ubuntu for AI development

## Hardware

- **Platform**:  [Qualcomm IQ-9075 EVK](https://www.qualcomm.com/developer/hardware/qualcomm-iq-9075-evaluation-kit-evk)

## Software & Toolkit

- **Qualcomm AI Runtime (QAIRT) SDK**：v2.44.0.260225
- **System:** Yocto

## Background & Solution

### Motivation

- Creating a One-Touch Toolkit to show Qualcomm Edge AI strength

### Solution

- One-touch PyTorch-to-QNN model conversion
- Live QNN inference on IQ-9075 EVK
- Performance Comparison: IQ-9075 EVK vs. Jetson Orin NX

## Architecture Diagram

The architecture diagram is divided into three phases, corresponding to the three colors in the legend on the left

Blue Phase: Convert the PyTorch model into a QNN model, and evaluate the benchmark for the QNN model

Purple Phase: Perform real-time inference and display the results using a USB camera based on the converted QNN model

Black Phase: Convert the PyTorch model to TensorRT on the NVIDIA Jetson Orin NX, and evaluate its benchmark to compare with the IQ-9075

![Architecture Diagram](assets/architecture.png)

## Results

![Self-built Dataset Benchmark: Surgical Instruments Detection](assets/results-surgical-instruments_1.png)

![Self-built Dataset Benchmark: Food Detection](assets/results-food-detection.png)

## Demo
https://github.com/user-attachments/assets/d5ef2402-10a8-4f7a-84e2-c983b28fdaaf


