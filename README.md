# CMPE258_HW2_YOLOv4

I used transfer learning to retrain the YOLOv4 model.
# Modified files:
## 1. cfg/yolov4-obj.cfg
  max_batches = 20000
  steps = 16000, 18000 
  classes = 10 in the three YOLO layers and filters = 45 in the three convolutional layers before the YOLO layers.
  width = 416
  height = 416
## 2. data/obj.names
  Apple
  Orange
  Pear
  Banana
  Strawberry
  Grape
  Grapefruit
  Pomegranate
  Mango
  Peach
## 3. data/obj.data
  classes= 10
  train  = data/train.txt
  valid  = data/test.txt
  names = data/obj.names
  backup = /mydrive/yolov4/backup
