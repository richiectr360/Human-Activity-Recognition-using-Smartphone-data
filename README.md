# Human Activity Recognition Using Smartphone Sensors

## Detailed Overview

This project harnesses the power of machine learning to interpret data from smartphone sensors, aiming to classify six distinct human activities: walking, walking upstairs, walking downstairs, sitting, standing, and laying. By analyzing the intricate patterns of accelerometer and gyroscope data, we unlock the potential to predict and understand user activities in real-time, paving the way for advancements in health monitoring, user interface design, and beyond.

## Comprehensive Methodology

- **Advanced Data Collection**: Utilized the UCI HAR Dataset, encompassing sensor signals (accelerometer and gyroscope) collected from 30 volunteers performing activities while carrying a waist-mounted smartphone.
- **Rigorous Data Preprocessing**: Implemented signal noise filtering, normalization, and windowing techniques to enhance the quality and relevance of the sensor data for predictive modeling.
- **Deep Exploratory Data Analysis (EDA)**: Employed statistical analyses and visualization techniques to unearth underlying patterns and relationships within the sensor data, focusing on the temporal and frequency domain features that distinguish each activity.
- **Sophisticated Predictive Modeling**: Applied a range of machine learning algorithms, from traditional models like Support Vector Machines (SVM) to complex ensemble methods and neural networks, optimizing each to achieve the highest classification accuracy.
- **Critical Model Evaluation**: Conducted a thorough evaluation using cross-validation and confusion matrices to assess the predictive accuracy and generalizability of each model, with a special focus on identifying the models that excel in differentiating between similar activities such as sitting and standing.

## Granular Datasets Description

The dataset comprises detailed recordings from smartphone sensors, meticulously annotated with the corresponding human activity. Key aspects include:
- **Sensor Signals**: 3-axial linear acceleration and angular velocity, captured at a constant rate of 50Hz.
- **Signal Preprocessing**: Signals were preprocessed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window).
- **Feature Vector**: From each window, a 561-feature vector was extracted, encompassing time and frequency domain variables.

## Detailed Key Findings

- **Sensor Data Insights**: The analysis revealed that accelerometer and gyroscope readings exhibit distinct patterns for dynamic activities (e.g., walking, walking upstairs/downstairs) compared to stationary activities (e.g., sitting, standing, laying), with dynamic activities showing greater variance and frequency domain fluctuations.
- **Importance of Feature Engineering**: Advanced features, particularly those derived from the Fourier Transform, significantly improved the model's ability to distinguish between similar activities, highlighting the critical role of feature engineering in sensor data analysis.
- **Superior Models**: The Random Forest and Gradient Boosting models outperformed other algorithms, achieving over 95% accuracy in activity classification. These models were particularly adept at handling the multi-dimensional nature of the sensor data and capturing the non-linear relationships between features and activities.
- **Challenges in Activity Differentiation**: The most challenging aspect was differentiating between activities with subtle differences in sensor readings, such as sitting vs. standing. Here, deep learning models like CNNs showed potential by leveraging the spatial relationships within the sensor data.
- **Real-world Application Viability**: The high accuracy of the top-performing models underscores the feasibility of deploying such models in real-world applications, from fitness tracking to patient monitoring in healthcare.
