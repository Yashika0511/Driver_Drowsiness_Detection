# Driver Drowsiness detection system

The objective of a “driver drowsiness detection system” is to monitor a driver's level of alertness and detect signs  of drowsiness or fatigue while driving. This is achieved through various sensors and algorithms that analyze the driver's behavior, such as eye movement in which it detect the decreasing ratio of the eye’s landmarks . The system alerts the driver when it detects signs of drowsiness, allowing the driver to take necessary measures to prevent accidents.

 The main aim of this system is to increase road safety by reducing the number of accidents caused by drowsy or fatigued drivers. 
 



## Algo
Step 1 – Take image as input from a camera.

Step 2 – Detect the face in the image and create a Region of Interest (ROI).

Step 3 – Detect the eyes from ROI and feed it to the classifier.

Step 4 – Classifier will categorize whether eyes are open or closed.

Step 5 – Calculate score to check whether the person is drowsy.

## Project prerequisites 

1. OpenCV – pip install opencv-python (face and eye detection).
2. TensorFlow – pip install tensorflow (keras uses TensorFlow as backend).
3. Keras – pip install keras (to build our classification model).
4. Pygame – pip install pygame (to play alarm sound).

## Dataset
The dataset used for this model is created by us. To create the dataset, we wrote a script that captures eyes from a camera and stores in our local disk. We separated them into their respective labels ‘Open’ or ‘Closed’. 

The data comprises around 7000 images of people’s eyes under different lighting conditions. 

Now, you can use this model to classify if a person’s eye is open or closed.

We are using this dataset:
 - [ Driver Drowsiness Dataset](https://www.kaggle.com/datasets/serenaraju/yawn-eye-dataset-new)


## Screenshots and testing

If the score<15 means the driver is not sleepy, if it get increased and reaches upto 15 or more than that ,the drowsiness get detected and it will beep alarm.
The alarm will get automatically stop when the score will reaches below 15 .
# output
![photo_2023-04-28_22-22-57](https://user-images.githubusercontent.com/88017738/235731820-ae9ba2e5-6830-4832-a85f-4fa68bc01466.jpg)
![photo_2023-04-28_22-23-13](https://user-images.githubusercontent.com/88017738/235731934-099b336c-9ed3-464b-aed8-f54b64cff7cb.jpg)

Our project can detect the eyes when the driver is wearing spectacles

![photo_2023-04-28_22-30-40](https://user-images.githubusercontent.com/88017738/235730974-390b9cc5-b1de-455e-80e0-0d4a855fb2e8.jpg)
![photo_2023-04-28_22-30-46](https://user-images.githubusercontent.com/88017738/235730989-27bf3383-8805-4327-a9c7-2b47b3c9bde6.jpg)

## Future scopes
● The system can be made more accurate using various other parameters such as State of the Car, Detecting Foreign Substances on Face etc.

● An application can be developed where it can alert or prevent the user from sleeping.

● It can be used to develop an IOT device that can be installed in the car to detect driver’s drowsiness. 

● Similar models and techniques can be used for various other uses such as Netflix, Hotstar and other streaming service platforms can detect whether the person is sleeping and stop the video accordingly.

