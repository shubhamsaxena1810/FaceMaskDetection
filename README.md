# FaceMaskDetection

This is a software which detects whether the user in front of the camera is wearing the mask or not, and if yes then how properly.
Here a scale of percentage from 1-100% is used to determine how properly is the user wearing the mask.

2 basic colours- RED and GREEN are used to depict the mask is proper or not.
The square box on the face of the user changes its colour on the **basis of accuracy**. 

The variations being:-

Accuracy | Colour | Message | Image
---------|--------|---------|--------------
1.**a<50%** | Red | *Wear the mask* | ![capture (2)](https://user-images.githubusercontent.com/61288929/115899391-53936280-a47c-11eb-817b-cc2bc7a58e79.jpg)
2.**50<=a<99%** | Green | *Wear the mask properly* | ![capture2](https://user-images.githubusercontent.com/61288929/115899413-57bf8000-a47c-11eb-94bc-e5cf222f9ab1.jpg)
3.**99% >= a** | Green | *The Mask is Proper* | ![capture3](https://user-images.githubusercontent.com/61288929/115899429-5d1cca80-a47c-11eb-9a1c-32068d1a63a7.jpg)
- - - -

The Model is trained on a dataset from kaggle:-

Directory Name | No. of Images | Training/Testing
---------------|---------------|-----------------
with_mask | 1532 | Training
with_mask | 383 | Testing
without_mask | 1534 | Training
without_mask | 384 | Testing

Technologies Used:-
1. tensorflow>=2.4.1
2. keras==2.3.1
3. imutils==0.5.3
4. numpy==1.18.2
5. opencv-python==4.2.0.*
6. matplotlib==3.2.1
7. scipy==1.4.1

Basic Data Augmentation techniques like rotation, zoom, height shift, width shift, shear range and horizontal flip were used.
**The Training Accuracy touches 99%**

Graph plot for Training And Validation loss and accuracy
![plot](https://user-images.githubusercontent.com/61288929/115892549-e16b4f80-a474-11eb-9e58-bcf18680de6b.png)

Thank you..
