# Hotel Reservation Cancellation
This repository is the Final Data Science Project at Dibimbing.id. This project contains the results of analysis of the dataset of hotel booking/reservation history observations related to predictions of prospective guests who cancel reservations. This analysis involves Exploratory Data Analysis (EDA) and Machine Learning Classification.

## Project Goals
The problem to be solved is related to hotel customer reservation cancellations. The main goal is to minimize the number of cancellations that occur, so that it can help increase room occupancy rates and hotel revenue.

### Why is it important to solve the problem?
Resolving/minimizing these issues can help:
1. Increase room occupancy and revenue levels
2. Help create efficient planning and reduce operational costs
3. Increase guest satisfaction and encourage loyalty
4. Strengthen competitive advantage by properly managing cancellation incidents

## Dataset
The dataset contains hotel booking history data between the 1st of July 2015 and 31st of August 2017, with a total of 119,390 observation records across 35 columns.
- Source: https://www.kaggle.com/datasets/mojtaba142/hotel-booking

## Methodology
- **Data Preprocessing:** Validating missing values, duplicate values, handling outliers, ensuring correct data types and remove extreme/anomalous data.
- **Feature Engineering:** feature selection, split dataset, categorical encoding, standardization, converting training data into numpy arrays
- **Model Evaluation:** The matrices used for the classification model are Precision, Recall, F1-Score, and Confusion Matrix. Recall is preferred to measure the proportion of positive data (cancelled reservations) that are actually classified as positive. This is intended to address potential revenue loss, prevent a decline in hotel reputation and staff performance and increased costs incurred by the hotel from changes in operational plans due to sudden cancellations. Accuracy is considered less relevant because the data is unbalanced (the number of cancellations is much less than the majority of non-cancellations)

## Result (Last Update)
- The prediction results of hotel reservation cancellation targets are more easily recognized through the Random Forest, XGBoost and LightGBM Model with a prediction accuracy above 90 percent.
- The results of Parameter Tuning from each model have been proven to be able to improve the prediction results for reservation cancellations on the following testing data (Recall):
1. Logistic Regression : 0.78 (Baseline)
2. Decision Forest: 0.88
3. **Random Forest: 0.90**
4. Support Vector Machine: 0.83
5. Neural Network (MLP): 0.85
6. **XGBoost: 0.95**
7. **LightGBM: 0.90**
- Key features based on model results for predicting reservation cancellations are more directed at the following factors:
1. **Availability of facilities:** required_car_parking_spaces and total_of_special_requests.
2. **Booking History Management:** reservation_status_date, days_in_waiting_list and is_repeated_guest.
   
## Business Recomendation
- Implement loyalty programs such as providing special offers, discounts, or room upgrades exclusively for loyal guests and conducting more personal communication.
- Optimize services especially during the season or holiday time.
- Conduct training for staff to provide better, friendlier, and more proactive service. Pay attention to small details that can increase guest satisfaction, such as providing additional facilities or special treatment. As well as fast and effective complaint management to minimize the negative impact on the hotel's reputation.
- Review the cancellation policy to offer more flexible cancellation options, especially for loyal guests.
- Provide incentives for guests who recommend the hotel to friends or family and conduct regular surveys to get direct feedback from guests.
- Consider the potential use of social media to interact with guests and build a community.

## Contact
**Author: Hudzaifah Rizqi Kamil**
- **Email:** hudzaifahrizqikamil@gmail.com
- **LinkedIn:** https://www.linkedin.com/in/hudzaifahrizqikamil
- **GitHub:** https://github.com/HudzaifahRizqi

Thank you for exploring this project! Suggestions, Feedback and contributions are welcome. Feel free to customize it further to suit your preferences!
