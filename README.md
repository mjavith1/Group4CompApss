1.	*Introduction*
   
Type 1 diabetes, a critical and challenging aspect of their care. Managing glucose levels is notoriously difficult due to the complex interplay of factors like diet, physical activity, and hormonal changes. The amount of insulin needed by a patient with Type 1 diabetes (T1D) depends on factors such as weight, age, physical activity, sickness, stress, and the type and timing of food consumed.
Incorrect insulin regulation can lead to hyperglycemia or hypoglycemia, making it critical for patients with T1D to accurately monitor their glucose levels. Any failure in regulation can be fatal.  Additionally, keeping blood sugar levels close to normal reduces the risk of many long-term complications. Given the challenges in predicting glucose levels, there is a clear need for a model capable of accurately forecasting blood glucose fluctuations.

2. *Dataset*

This data set is from a study that collected data from young adults in the UK with type 1 diabetes, who used a continuous glucose monitor (CGM), an insulin pump and a smartwatch. These devices collected blood glucose readings, insulin dosage, carbohydrate intake, and activity data. The data collected was aggregated to five-minute intervals and formatted into samples. Each sample represents a point in time and includes the aggregated five-minute intervals from the previous six hours. The aim is to predict the blood glucose reading an hour into the future, for each of these samples. The data itself is complex given that it is medical data. Thus, there were missing values and noise in the data that we had to consider while preprocessing. 

Competition: Sam Gordon James, Miranda Elaine Glynis Armstrong, Aisling Ann O'Kane, Harry Emerson, and Zahraa S. Abdallah. BrisT1D Blood Glucose Prediction Competition. https://kaggle.com/competitions/brist1d, 2024. Kaggle.

3.	*Methods*

General Overview:

1. Uploading data ZIP file
   Once you download the data, you must change the portion in the code to correctly link to the filepath where you saved the downloaded csv files. You can copy and paste your filepath directly into the notebook.

2. Preprocessing Data
   
   2.1 Generate descriptive statistics
   
   2.2 Reducing memory usage
   
   2.3 encoding categorical variables
   
   2.3 fit and transform categorical colums
   
   2.4 drop colums with more than 60% of missing values
   
   2.5 drop columns with low variance
   
   2.6 standardize and fill in missing values using KNNImputer
   
   2.7 eliminate outliers using IQR method
   

3. Create ANN and Linear Regression Models

4. Use Matplotlib to plot results of model efficacy
   
   4.1 Model Loss Evaluation
   
   4.2 Prediction Error Plot
   
   4.3 Histogram of Residuals

   4.4 ANN Model Predictions vs Actual
   
   4.5 Receiver Operating Characteristic (ROC) Curve


Prediction Models:

-ANN

-Linear Regression

5.	*Results*
   
   ![image](https://github.com/user-attachments/assets/6d392171-d76f-4c94-8503-c55ed0780404)

  ![image](https://github.com/user-attachments/assets/5416511d-bd26-43d3-a62f-0e9a55178e88)
  ![image](https://github.com/user-attachments/assets/db88d183-799e-4f96-8c28-c7a136b95163)


