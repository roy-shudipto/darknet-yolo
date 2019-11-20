# darknet-yolo

## Required: 
Linux, CUDA, CUDNN, OpenCV

## Instructions:
- Default settings are for Turing architecture and CUDA 10.0
- If the architecture is other than Turing: 
  - Modify the darket-yolo/Makefile: Use ARCH for CUDA 9.0 
  - Modify the darket-yolo/cfg/yolov3.cfg: batch=16 
- Open a terminal in the darket-yolo directory and run: make

## Download Pre-Trained weight file:
wget https://pjreddie.com/media/files/yolov3.weights

## Test with: 
./darknet detector test cfg/coco.data cfg/yolov3.cfg yolov3.weights data/dog.jpg
