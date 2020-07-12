# Car damage detector 

### This application is made to detect which part of car is damaged 

#### To quickly view final results open [Final output]() and scroll to the bottom 


#### Dataset:  
- Training set: 62 images  
- Validation set: 8 images  
- Test set: 8 images

#### Approach:

The nature of annotations in the dataset and its small size make segmentation a good option.  
[FPN](http://presentations.cocodataset.org/COCO17-Stuff-FAIR.pdf) model available in pytorch is used. Initialised with ResNet weights for feature extraction  
Two segmentation models are trained:
  1. To give which parts of car body are in image  
  This model is trained on the 5 parts tagged in the annotations 
  2. To give which area is damaged 
  
IOU over these two results tells us which body part was damaged.

On test set of 8 images, 7 are classified correctly.

#### Further:  



