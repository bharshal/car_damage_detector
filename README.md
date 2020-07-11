# car_damage_detector
Detecting which part of car is damaged. 

Method used is segmentation due to nature of data.

Two segmentation models are trained:
  1. To give which parts of car body are in image 
  2. To give which area is damaged 
  
IOU over these two results tells us which body part was damaged.

On test set of 8 images 7 are classified correctly. 


