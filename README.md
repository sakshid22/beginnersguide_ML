# A Beginner's Guide to Machine Learning 
Welcome to the first session of the Tech Talk Series presented by Honeywell's Women Network. This github page is dedicated to kick start your first ML session. We will be running python scripts to recognize hand written digits.
Handwritten Digit Recognition will be done using OpenCV, sklearn and Python

# Environment
1. Python
2. R

# Dependencies
1. `cv2`
2. `sklearn`
3. `skimage`
4. `numpy`
5. `collections`

# Contents
This repository contains the following files-

1. `generateClassifier.py` - Python Script to create the classifier file `digits_cls.pkl`.
2. `performRecognition.py` - Python Script to test the classifier.
3. `digits_cls.pkl` - Classifier file for digit recognition.
4. `photo_1.jpg` - Test image number 1 to test the classifier
5. `photo_2.jpg` - Test image numbre 2 to test the classifier

## Usage 

* Clone the repository - 
```bash
cd 
git clone https://github.com/sakshid22/beginnersguide_ML.git
cd beginnersguide_ML-master
```
* The next step is to train the classifier. To do so run the script `generateClassifier.py`. It will produce the classifier named `digits_cls.pkl`. 

**NOTE** - *I have already created the `digits_cls.pkl`, so this step is not necessary.*
```python
python generateClassifier.py
```
* To test the classifier, run the `performRecognition.py` script.
```python
python performRecognition.py -c <path to classifier file> -i <path to test image>
```
ex -
```python
python performRecognition.py -c digits_cls.pkl -i photo_1.jpg
```

## Results

### Sample Image 1
![Result Number 1](http://hanzratech.in/figures/digit-reco-1-out.png)
### Sample Image 2
![Result Number 2](http://hanzratech.in/figures/digit-reco-2.png)

## TODO

* Add a CNN Based approach
* Reject bounding boxes lesser than some area
* Look into user errors

Data Credites: bikz05, Kaggle.
