# Food-Detector
A Food Detector Project created using YoloV5 and PyTorch run Jetson Nano

## Hardware Required
1. Jetson Nano
2. Mouse and Keyboard
3. Logitech C270 HD Webcam
4. Wifi Adapter

## Create a new environment with Python Version 3.8
$ conda create -n myenv python=3.8

Managing environment guides [here](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#viewing-a-list-of-your-environments)

## Installation

1. Clone the YoloV5 repo
   - $ git clone https://github.com/ultralytics/yolov5
   - $ cd yolov5
   - $ pip install -r requirements.txt
   
2. Modify requirements.txt
   - Locate and open YoloV5 directory
   - Open requirements.txt using text editor
   - Comment #torch>=1.7.0 #torchvision>=0.8.1

3. Install PyTorch
   - $ git clone --recursive --branch 1.7 http://github.com/pytorch/pytorch
   - $ cd pytorch
   - $ python3.8 -m pip install -r requirements.txt
   - $ python3.8 setup.py install

4. Install torchvision
   - $ git clone https://github.com/pytorch/vision
   - $ cd vision/
   - $ git checkout v0.8.
   - $ python3 setup.py bdist_wheel
   - $ python3 -m pip install dist/torchvision-0.8.0a0+291f7e2-cp38-cp38-linux_aarch64.whl

## Check GPU
1. cd to HOME
2. Activate python3 by inserting $ python3
3. $ import torch
4. $ torch.cuda.is_available()
5. $ torch.cuda.current_device()
6. $ torch.cuda.device(0)
7. $ torch.cuda.device_count()
8. $ torch.cuda.get_device_name(0)


## Run the Inferences using webcam
$ python detect.py --weights food.pt --source 0

## Thank You
Thank you for all the lecturers, facilitators, friends and family for helping me to develop the project. Any kind of improvement or suggestions are most welcomed.
