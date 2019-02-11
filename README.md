# Fingerprint Recognition
Fingerprint recognition using CNN  

## Result

![result.png](https://github.com/kairess/fingerprint_recognition/raw/master/result/result.png)  
Let's assume that left image is a new input from user, center and right images are stored in database.  
Title of figures [122 0 0 1] means, left to right order:  
- subject_id
- gender (male 0, female 1)
- left_or_right_hand (left 0, right 1)
- finger index (0-4)
  
Applied some augmentation(gaussian blur, zoom, translation, rotation..) to input(left image) for wild environment.  
Center image is the answer so it has 99% confidence, on the other hand, right image is wrong so that has 0%.  

## Model Architecture
![model.jpg](https://github.com/kairess/fingerprint_recognition/raw/master/result/model.jpg)  

## Dependencies
- Python
- numpy
- keras
- matplotlib
- sklearn
- [imgaug](https://github.com/aleju/imgaug)

## Dataset

Sokoto Coventry Fingerprint Dataset (SOCOFing) https://www.kaggle.com/ruizgara/socofing/home
