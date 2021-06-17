# Human Activity Recognition using smartphone data

![git 1](https://user-images.githubusercontent.com/71088477/122425540-2f03c480-cfad-11eb-9d1f-347b3e3a263d.jpg)

Ever wondered how your smartphone, smartwatch or wristband knows when you’re walking, running or sitting? Well, your device probably has multiple sensors that give various information.

## Project Overview
- Human Activity Recognition, or HAR for short, is the problem of predicting what a person is doing based on a trace of their movement using sensors.
- The project is to build a model that predicts the human activities such as walking, walking upstairs, walking downstairs, sitting, standing or laying.
- The dataset we will work on is collected from 30 persons(referred as subjects in the dataset), performing differengt activities with a smartphone to their waists.
- The data is recorded with the help of sensors (accelerometer and Gyroscope) present in the smartphone.
- This experiment was video recorded to label the data manually.
- Readings are divided into a window of 2.56 seconds with 50% overlapping.
- Accelerometer readings are divided into gravity acceleration and body acceleration readings, which has x,y and z components each.
- Gyroscope readings are the measure of angular velocities which has x,y and z components.
- Jerk signals are calculated for BodyAcceleration readings.
- Fourier Transforms are made on the above time readings to obtain frequency readings.
- Now, on all the base signal readings, mean, max, mad, sma, arcoefficient, engerybands,entropy etc., are calculated for each window.
- We get a feature vector of 561 features and these features are given in the dataset.
- Each window of readings is a datapoint of 561 features.

## How data was recorded ?
![5](https://user-images.githubusercontent.com/71088477/122425330-0976bb00-cfad-11eb-806c-47654efe1888.png)
- By using sensors
    - Gyroscope
    - Accelerometer
- Collected by using sensors which are present in smartphone
- They have captured '3-axial linear acceleration'(tAcc-XYZ) from accelerometer and '3-axial angular velocity' (tGyro-XYZ) from Gyroscope with several variations.
    - Prefix t in the feature denotes time
    - Suffix 'XYZ' represnts 2 axial signals in X, Y and Z directions

## Problem Framework¶
- 30 subjects(volunteers) data is randomly split to 70%(21) test and 30%(7) train data.
- Each datapoint corresponds one of the 6 Activities.

## Problem Statement
Given a new datapoint, we have to predict the Activity

