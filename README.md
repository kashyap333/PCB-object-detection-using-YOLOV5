# PCB-object-detection-using-YOLOV5

Implementation of Faster RCNN and RESNET using Tensorflow object detection api2 for PCB component detection like resistors, capacitors etc.
This repository also contains custom scripts for the following:
  1. Visualisation of the bounding boxes.
  2. Extracting bounding boxes and saving them folder named after the image and with folder for each individual images for further implementation of OCR on the components
  3. Optical Character Recognition using easyOCR

### Installation of the Object detection api

The complete installation and setup can be found at "(https://github.com/ultralytics/yolov5.git)"

### Database

FICS-PCB: A MULTI-MODAL IMAGE DATASET FOR AUTOMATED PRINTED CIRCUIT BOARD VISUAL INSPECTION
link: "https://www.trust-hub.org/#/data/fics-pcb"

### Data preparation

csv files are modified into txt format to be compatible with YOLOV5


### Results

best.pt is the inference model, for direct inference.

![s12_front (Medium)](https://user-images.githubusercontent.com/38318593/170716237-f5f86dd6-b047-41fb-9283-ce61fddd068c.jpg)
![s12_front (Medium)](https://user-images.githubusercontent.com/38318593/170716313-077f4788-e566-4b89-8024-892250ac19be.jpg)

### Notes and suggestions

1. Ensure gpu installation for running smoothly and quickly: I have included my pc specs below for comparison
2. Things you should do to improve results, which I could not because of memory constraints:
    1. Increase batch size to improve batch normalisation
    2. Give model a higher resolution image froom the dataset as the components are very small 
    3. Play aound with the learning rate
3. Get more images. This dataset of 50 is very samll for any meaningfull success, if you get more images, highly appreciate if you do share it with me at "kashyapmahesh97@gmail.com"

### PC specs
1. CPU: Intel(R) Xeon(R) W-3223 CPU
2. Ram: 64 gb ddr4
3. GPU: Nvidia RTX quadro 4000 (8gb vram)
