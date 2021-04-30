# CMPE258_HW2_YOLOv4

# I used transfer learning to retrain the YOLOv4 model.
# 2000 images for training and 200 for validation.

# Modified files:
## 1. cfg/yolov4-obj.cfg
  max_batches = 6000
  steps = 4800, 5400 
  classes = 2 in the three YOLO layers and filters = 21 in the three convolutional layers before the YOLO layers.
  width = 416
  height = 416
## 2. data/obj.names
  Apple
  Orange
## 3. data/obj.data
  classes= 2
  train  = data/train.txt
  valid  = data/test.txt
  names = data/obj.names
  backup = /mydrive/yolov4/backup

