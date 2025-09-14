# Sleep Health Data Analysis

![insomnia](https://github.com/user-attachments/assets/0cfd9dab-3ed0-444e-bfa9-b7084ba37c11)

## Discovering Insights into Sleep Quality

SleepInc, has shared anonymized data from their popular sleep tracking app, SleepScope. My mission is to analyze this lifestyle survey data to discover relationships between factors like exercise, gender, occupation, and sleep quality. This analysis aims to identify patterns that provide insights into what affects sleep health.

## 💾 The Dataset: `sleep_health_data.csv`

SleepInc provided an anonymized dataset of 374 individuals containing sleep and lifestyle metrics. This dataset includes average values for each person calculated over the past six months.

| Column | Description |
|---|---|
| `Person ID` | An identifier for each individual. |
| `Gender` | The gender of the person (Male/Female). |
| `Age` | The age of the person in years. |
| `Occupation` | The occupation or profession of the person. |
| `Sleep Duration (hours)` | The average number of hours the person sleeps per day. |
| `Quality of Sleep (scale: 1-10)`| A subjective rating of the quality of sleep, ranging from 1 to 10. |
| `Physical Activity Level (minutes/day)`| The average number of minutes the person engages in physical activity daily. |
| `Stress Level (scale: 1-10)`| A subjective rating of the stress level experienced by the person, ranging from 1 to 10. |
| `BMI Category` | The BMI category of the person (e.g., Underweight, Normal, Overweight). |
| `Blood Pressure (systolic/diastolic)`| The average blood pressure measurement of the person. |
| `Heart Rate (bpm)`| The average resting heart rate in beats per minute. |
| `Daily Steps`| The average number of steps the person takes per day. |
| `Sleep Disorder`| The presence or absence of a sleep disorder (None, Insomnia, Sleep Apnea). |

## Analysis and Findings

The data analysis focused on answering key questions about the relationship between occupation, BMI, and sleep quality.

### 1\. Occupation with the Lowest Sleep Quality and Duration

The first analysis aimed to identify which profession gets the least amount of sleep, both in terms of duration and quality.
The data was grouped by `Occupation` to calculate the average `Sleep Duration` and `Quality of Sleep`. The results show that **Sales Representative** is the occupation with both the **lowest average sleep duration** and the **lowest average sleep quality**.

### 2\. Relationship Between BMI and Insomnia

Next, i investigated whether there is a connection between a person's Body Mass Index (BMI) category and their likelihood of suffering from insomnia.
By grouping the data by `BMI Category` and `Sleep Disorder`, i calculated the ratio of individuals experiencing Insomnia in each category. The analysis found a strong correlation:

  * **Normal**: Only **4%** of individuals in this category reported Insomnia.
  * **Overweight**: This ratio jumped dramatically to **43%**.
  * **Obese**: The ratio was slightly lower but still very significant at **40%**.

This finding indicates that individuals in the 'Overweight' and 'Obese' BMI categories are far more likely to suffer from insomnia compared to those with a normal weight.

## Conclusion

This analysis provides crucial insights for SleepInc. The **Sales Representative** profession was identified as a group at high risk for sleep-related issues, concerning both duration and quality. Furthermore, a clear link was established between a **higher BMI** and an **increased risk of insomnia**. These insights can be used to develop targeted app features or wellness programs to help specific user groups improve their sleep health.

## Tools Used

  * **Python**
  * **Pandas**
