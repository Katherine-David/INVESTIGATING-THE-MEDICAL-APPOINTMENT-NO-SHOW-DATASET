# INVESTIGATING THE MEDICAL APPOINTMENT NO-SHOW DATASET

## INTRODUCTION
The **"Medical Appointment No Shows"** dataset from Kaggle provides a comprehensive record of medical appointments in Brazil, focusing on whether patients attended their scheduled appointments. This dataset contains valuable information, including patient demographics, appointment details, and medical history, which can be used to gain insights into factors influencing patient attendance. By analyzing this dataset, we aim to uncover trends and patterns that can help healthcare providers improve appointment scheduling and patient care strategies.

## OBJECTIVES
The primary objective of the investigation was to identify key factors or features that could predict whether a patient would show up for their scheduled appointment.

## DATASET DESCRIPTION

**Data Source**:[No-Show Appointment Dataset] https://www.kaggle.com/datasets/joniarroba/noshowappointments

The medical appointment dataset contains information about 110,527 medical appointments of different patients in different hospitals in Brazil.The dataset shows the number of appointments showed up for and the ones missed. It also has 14 variables which tell us about the patient and helps to predict if the patient will show up for the appointment or not. The 14 variables or characterisctics called data dictionary are:

**Patient ID:** Identification of patient. \
**Appointment ID:** Identification of each appointment. \
**Gender:** Male or Female . Female is the greater proportion, woman takes way more care of they health in comparison to man. \
**Appointment Day:** The day of the actual appointment, when they have to visit the doctor. \
**Scheduled Day:** The day someone called or registered the appointment, this is before appointment of course. \
**Age:** How old is the patient. \
**Neighbourhood:** Where the appointment takes place. \
**Scholarship :** True or False.Scholarship indicates whether or not the patient is enrolled in Brazilian welfare program Bolsa Família. \
**Hypertension:** True or False. \
**Diabetes:** True or False. \
**Alcoholism:** True or False. \
**Handicap:** True or False. \
**SMS_received:** 1 or more messages sent to the patient. \
**No-show:** True or False. 

## METHODOLOGY
* The dataset was sourced from Kaggle, specifically from the dataset "Medical Appointment No Shows" by Joni Hoppen and Aquarela Advanced Analytics.
* It was downloaded securely, ensuring compliance with data privacy regulations.
* The dataset was explored to understand its structure and identify any anomalies.
* Data cleaning operations were performed, including handling missing values and removing duplicates.
* Unnecessary columns or features were trimmed from the dataset.
* The research question focused on investigating the factors or features that are important in predicting if a patient will show up for their scheduled appointment.
* Statistical and visual analysis techniques were used to explore relationships between different features and the target variable.

## DATA ANALYTICS TOOL
 Python in Jupyter Notebook 

## INSIGHTS
* Patients without hypertension are more likely to attend their appointments, but the percentage of patients with hypertension who attend is significantly higher than those who do not. This suggests that hypertension may influence appointment attendance.

* Diabetes patients have a high attendance rate compared to non-diabetes patients, indicating a serious commitment to medical appointments. This characteristic can be a reliable predictor of patient attendance.

* While the number of missed appointments by handicapped patients is low compared to those attended, the overall low number of handicapped patients in the dataset limits the predictive value of this characteristic.

* Similarly, although the number of missed appointments by alcoholic patients is low compared to those attended, the overall low prevalence of alcoholism in the dataset limits its predictive value.

* The dataset indicates a higher proportion of female patients than male patients. However, the attendance and no-show rates between genders are comparable, suggesting that gender is not a determining factor in predicting appointment attendance.

* The scholarship program enrollment status does not appear to predict whether a patient will show up for their appointment. Only 20 percent of patients on scholarships and 20 percent of those not on scholarships missed their appointments. Other variables likely play a more significant role in predicting attendance.

* Receiving an SMS notification does not seem to affect patient attendance. The number of patients who did not receive an SMS and missed their appointments is similar to those who received an SMS and also missed their appointments.

* Adults have the highest attendance rate compared to other age groups. This suggests that adults, along with children and seniors, tend to schedule more hospital appointments than youths. The higher attendance among adults and seniors may indicate a greater concern for their health. Children, who are typically accompanied by adults, also contribute to this trend. Therefore, age could be a significant factor in predicting attendance.

* Patients are more likely to show up for appointments on Monday, Tuesday, and Wednesday. Attendance drops towards the end of the week, with Thursday and Friday having moderate attendance. Few appointments are scheduled and attended on weekends (Saturday and Sunday), possibly due to people engaging in rest, cleaning, religious activities, or social events. Thus, the appointment's scheduled day of the week could be a useful predictor of attendance.

* Neighborhood data does not seem to be a reliable predictor of appointment attendance. The dataset's neighborhood information does not provide clear insights into whether a patient will show up for their medical appointment.

## CONCLUSION
Most of the patients in Brazil recorded in the dataset are females.The age-group of most patients scheduled for appointments ranges between adults and seniors. Some areas have more patients than others ,this can be due to the population of citizens in those areas.Some patients have terminal diseases which encouraged the patient to come for treatment ,most especially if its at the critical stage or in combination with other diseases such as hypertension. The exploratory analysis confirmed that correlation does not imply causation,example is the case of the relationship between SMS received and number of appointments showed up for which was contrary to what was expected. The age of patient,the week day of appointment and the hypertension status of the patient are important factors that can predict if a patient will show up for their appointment or not.

**LIMITATIONS:** The severity of the terminal disease was not given,having a disease might not be the reason of a patient going to the hospital except in a critical stage. Since some patients had appointment more than once,they might receive SMS motification at the second or third appointment if they missed or did not missed their first appointment and this was not captured for each patient properly in the dataset and thus affect the number of no_shows of SMS received in the dataset.

