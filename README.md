# Custom YOLOv9 License Plate Detection

This repository contains a comprehensive Google Colab notebook for training and deploying a custom object detection model using the YOLOv9 (GELAN-C) architecture.

## Project Overview
The goal of this project is to accurately detect vehicle license plates in static images. It leverages transfer learning on the GELAN-C architecture to achieve high accuracy with efficient training times.

## Key Features

1. Automated Environment Patching: Includes custom scripts to patch YOLOv9 source code for compatibility with the latest PyTorch 2.6+ security updates (resolving pickle.UnpicklingError issues).

2. Roboflow Integration: Seamlessly downloads and formats datasets from Roboflow Universe.

3. Path correction: Automatically fixes relative path issues in YOLO configuration files that frequently cause failures in cloud environments.

4. ONNX Export: Includes a dedicated step to export the trained model to .onnx format, making it ready for production deployment using ONNX Runtime or FastAPI.

## Workflow

1. Setup: Install dependencies & patch source code.

2. Data: Ingest data via Roboflow API.

3. Train: Fine-tune YOLOv9 for 25+ epochs.

4. Test: Batch inference on sample images.

5. Deploy: Export model weights for downstream applications.
