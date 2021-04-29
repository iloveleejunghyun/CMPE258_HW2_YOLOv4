# CMPE258_HW2_YOLOv4

# I used transfer learning to retrain the YOLOv4 model.
# 2000 images for training and 200 for validation.

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

# Results: I spent over 7 hours to train the model but it only can detect Apple and Orange. I think it's because there're too many images to train and the performance of Google Colab is limited.
![Image text]([https://github.com/iloveleejunghyun/CMPE258_HW2_YOLOv4/blob/main/1.PNG])
