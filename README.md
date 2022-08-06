# Food-Detector
A Food Detector Project created using YoloV5 and PyTorch run Jetson Nano

## Hardware Required
1. Jetson Nano
2. Mouse and Keyboard
3. Logitech C270 HD Webcam
4. Wifi Adapter

## Create a new environment with Python Version 3.8
$ conda create -n myenv python=3.8

## Installation

1. Clone the YoloV5 repo
   - git clone https://github.com/ultralytics/yolov5
   - cd yolov5
   - pip install -r requirements.txt
   
2. Modify requirements.txt
   - Locate and open YoloV5 directory
   - Open requirements.txt using text editor
   - Comment #torch>=1.7.0 #torchvision>=0.8.1
