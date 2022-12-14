# π Cardiovascular-risk-prediction - Manas Ranjan Behera

![a hologram](https://user-images.githubusercontent.com/103633582/208310760-4b0abbc7-e253-4d57-8d0c-5364bfae80fc.jpeg)

## π Introduction -

Heart disease is the major cause of morbidity and mortality globally: it accounts for more deaths annually than any other cause. According to the WHO, an estimated 17.9 million people died from heart disease in 2016, representing 31% of all global deaths. Over three quarters of these deaths took place in low- and middle-income countries.

Of all heart diseases, coronary heart disease (aka heart attack) is by far the most common and the most fatal. In the United States, for example, it is estimated that someone has a heart attack every 40 seconds and about 805,000 Americans have a heart attack every year (CDC 2019).

Doctors and scientists alike have turned to machine learning (ML) techniques to develop screening tools and this is because of their superiority in pattern recognition and classification as compared to other traditional statistical approaches.

In this project, We will be giving you a walk through on the development of a screening tool for predicting whether a patient has a 10-year risk of developing coronary heart disease(CHD) using different Machine Learning techniques.

# π Data Summary -

The dataset is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD). The dataset provides the patientsβ information. It includes over 4,000 records and 15 attributes.Each attribute is a potential risk factor. There are both demographic, behavioral, and medical risk factors.

## π Data Description Demographic - 

β’ Sex: male or female("M" or "F") 

β’ Age: Age of the patient;(Continuous - Although the recorded ages have been truncated to whole numbers, the concept of age is continuous) Behavioral 

β’ is_smoking: whether or not the patient is a current smoker ("YES" or "NO") 

β’ Cigs Per Day: the number of cigarettes that the person smoked on average in one day.(can be considered continuous as one can have any number of cigarettes, even half a cigarette.) Medical( history) 

β’ BP Meds: whether or not the patient was on blood pressure medication (Nominal) 

β’ Prevalent Stroke: whether or not the patient had previously had a stroke (Nominal) 

β’ Prevalent Hyp: whether or not the patient was hypertensive (Nominal) 

β’ Diabetes: whether or not the patient had diabetes (Nominal) Medical(current) 

β’ Tot Chol: total cholesterol level (Continuous) 

β’ Sys BP: systolic blood pressure (Continuous) 

β’ Dia BP: diastolic blood pressure (Continuous) 

β’ BMI: Body Mass Index (Continuous) 

β’ Heart Rate: heart rate (Continuous - In medical research, variables such as heart rate though in fact discrete, yet are considered continuous because of a large number of possible values.) 

β’ Glucose: glucose level (Continuous) Predict variable (desired target) 

β’ 10-year risk of coronary heart disease CHD(binary: β1β, means βYesβ, β0β means βNoβ) - DV

## π Results:

|Model Name|Recall|Accuracy|F1-score|

|Logistic regression|0.68|0.67|0.38| 

|KNN| 0.63|0.49|0.29| 

|SVM| 0.64|0.74|0.38|

## π Conclusion

We have used Logistic Regression, KNN, SVC and XGBoost for modelling. Based on our observations, the Support vector classifier seems to have performed better with a recall of 74%. Based on the recall metrics, the model performance is really good, which was our objective from the very beginning i.e. we wanted to correctly predict all the positive cases of high risk CHD.

However, we sometimes also donβt want to flag somebody with no risk of CHD as positive, which might eventually increase the operational cost. We need to ensure that our precision is not too low as well.Thats where our best model still lags. The current precision of the SVC model is around ~0.26. Further work needs to be done that might possibly improve the precision of our model on minority class as well.
