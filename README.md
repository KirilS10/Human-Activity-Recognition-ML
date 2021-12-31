# Human-Activity-Recognition-ML
This project provides opportunity to apply Machine Learning algorithms on human generated data to automatically detect human activities. The project is based on the collected and logged sensor data which include three activities such as: walking, jumping and drop and pickup object. All data from three activities were manually recorded and collected by phone in home-based environment. 
# Framework Description
The activity recognition steps are included: (a) the load acceleration, magnetic field, orientation and angular velocity data for all three activates collected from the smartphone, (b) the exploratory data analyse and visualisation steps, and (c) the classification algorithm. 
# Collecting Data and Data Pre-Processing
Data for all three activities (Walking, Jumping and Drop & Pick Up) were obtained from the acceleration, magnetic field, orientation and angular velocity sensors of the iPhone 11 Pro Max!During two activities (Walking and Jumping) the iPhone was attached to the body of the participant to gather acceleration, magnetic field, orientation and angular velocity data (see the sample in Figure 1 and Figure 2). However, the third activity was to drop the iPhone from the table (Height: 90 cm) and placed it back and repeat the action (see the sample in Figure 3). The MATLAB application was used to collect the sensor data from the iPhone. All three activities were logged for two (2) minutes and thirty (30) seconds with the sampling frequency of 20 Hz (One hertz is a unit of measurement that equals one cycle per second).

![image](https://user-images.githubusercontent.com/76842663/147565297-081311dd-e933-430d-be83-16c63ae091e0.jpeg)![image](https://user-images.githubusercontent.com/76842663/147565302-4470bf61-2db8-4fdc-af55-2b78ef95dcb8.jpeg)![image](https://user-images.githubusercontent.com/76842663/147565315-689106de-0b24-4dfb-80f6-afa60fbf434f.jpeg)

During two (2) minutes and thirty (30) seconds for each activity, the iphone’s sensors collected a total of 120,568 data points (8612 rows x 15 columns, including Timestamp and Activity columns)
# Data Visualization 
As we can see the plots(below) shows the acceleration plot which includes all three vectors (x,y,z) for each of the three activities. According to the plots with comparison to other activities, jumping is one of the most energetic activity with clear significant values. However the walking activity is also considered as energetic activity but the graph indicates that the all three vectors (x,y,z ) are more stable and constant . The plot for drop and pickup activity illustrates the dramatic spikes which are linked to our data. Due to the spikes, we are able to analyze that the vector (z) values have more dramatic acceleration. 
![image](https://user-images.githubusercontent.com/76842663/147565745-963972a7-6979-4c64-a150-28585794f725.jpeg)

Additionally, the next plot represents the angular velocity sensor for all three activities (Walking, Jumping and Drop & Pickup) including the three vectors (X, Y and Z). Due to the plots, we are able to identify large spikes on the drop and pickup activity sensor plot. The spikes illustrate the exact moment of time when the subject (iPhone) was dropped. However, for all three activities (Walking, Jumping and Drop & Pickup), the all three vectors showed significant changes. 
![image](https://user-images.githubusercontent.com/76842663/147565895-66adf347-3f03-4cc8-b97c-baec21d4a4e6.jpeg)
# Building ML modelS and learning process
The train-test split process includes taking the master dataset and splitting it into two subsets. The train dataset / subset is applied to fit the machine learning model. The test dataset / subset is used to evaluate the model performance and to made the predictions at the end of learning process. The main purpose of the test dataset its to measure the success of the machine learning algorithm on new data which was not used to train the machine learning model.

<img width="452" alt="image" src="https://user-images.githubusercontent.com/76842663/147566364-ae069652-1190-4a25-8d6e-f19f48b3adc6.png">

One of the important elements in the Activity Recognition project is classification algorithm applied to classify individual actions and activities focused on the data which was collected by user. 

In the Human Activity Recognition project, the performance of four Machine Learning algorithms were evaluated. The following classifiers were applied to train the model: Logistic Regression, K – Nearest Neighbor (KNN), Decision Tree and Random Forest. The classification algorithms were trained and tested by using Hyperparameters tuning and cross validations techniques.

# Results
<img width="792" alt="Screenshot 2021-12-28 at 12 34 05" src="https://user-images.githubusercontent.com/76842663/147566749-e2192b64-ec47-4bae-b115-2a2501687034.png">

In this project, the confusion matrixes for all four models were applied to summarise the performance of the classification models.
<img width="890" alt="Screenshot 2021-12-28 at 12 41 21" src="https://user-images.githubusercontent.com/76842663/147567350-b9d90137-12ae-4166-b4fc-55e0228443b4.png">

Our confusion matrixes for Multi-Class Classifications do not represent positive or negative classes. However, we are still able to calculate the result of prediction for each activity with True-Positive (Result which was predicted Positive and it is actually Positive), True-Negative (Result which was predicted Negative and it is actually Negative), False-Positive (Result which was predicted as Positive but it is actually Negative) and False-Negative (Result which was predicted as Negative and it is actually Positive) values.


