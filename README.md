# Brain_Stoke_Prediction
About Dataset
Story of dataset:
You can reach the original source of the data from the link.
https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset
<br>
While working on this data, there were 210 missing data available in a single numeric column. I've tried handling missing values, treating this just like a regression problem. I got some very interesting results. And I have even seen a similar designation in one of the top-rated notebooks, but there had been no performance evaluation for this designation and I considered it a shortcoming. Then considering R_square, I thought that the pipeline-based data assignment actually had a very low result and shouldn't even be considered a regression because the result was less than 0.3 : <br>

Instead, I found the most suitable algorithms (GradientBoostingRegressor, CatBoost, Light_GBM, and XGBoost) for a similar assignment with PyCaret, optimized it with optuna, and then developed a model using the blend method. <br>

Validation data values with this model; <br>
R_sqr: 0.3035774217245104
MSE: 32.60242593653817
I know still low, but this model showed the highest performance among all models. Then I wanted to make it available to all Kagglers. <br>

In terms of model estimation, you can try my previous notebook: My notebook <r>

## Context: 
<br>
A stroke is a medical condition in which poor blood flow to the brain causes cell death. There are two main types of stroke: ischemic, due to lack of blood flow, and hemorrhagic, due to bleeding. Both cause parts of the brain to stop functioning properly. Signs and symptoms of a stroke may include an inability to move or feel on one side of the body, problems understanding or speaking, dizziness, or loss of vision to one side. Signs and symptoms often appear soon after the stroke has occurred. If symptoms last less than one or two hours, the stroke is a transient ischemic attack (TIA), also called a mini-stroke. A hemorrhagic stroke may also be associated with a severe headache. The symptoms of a stroke can be permanent. Long-term complications may include pneumonia and loss of bladder control. <br>

The main risk factor for stroke is high blood pressure. Other risk factors include high blood cholesterol, tobacco smoking, obesity, diabetes mellitus, a previous TIA, end-stage kidney disease, and atrial fibrillation. An ischemic stroke is typically caused by blockage of a blood vessel, though there are also less common causes. A hemorrhagic stroke is caused by either bleeding directly into the brain or into the space between the brain's membranes. Bleeding may occur due to a ruptured brain aneurysm. Diagnosis is typically based on a physical exam and supported by medical imaging such as a CT scan or MRI scan. A CT scan can rule out bleeding, but may not necessarily rule out ischemia, which early on typically does not show up on a CT scan. Other tests such as an electrocardiogram (ECG) and blood tests are done to determine risk factors and rule out other possible causes. Low blood sugar may cause similar symptoms. <br>

Prevention includes decreasing risk factors, surgery to open up the arteries to the brain in those with problematic carotid narrowing, and warfarin in people with atrial fibrillation. Aspirin or statins may be recommended by physicians for prevention. A stroke or TIA often requires emergency care. An ischemic stroke, if detected within three to four and half hours, may be treatable with a medication that can break down the clot. Some hemorrhagic strokes benefit from surgery. Treatment to attempt recovery of lost function is called stroke rehabilitation, and ideally takes place in a stroke unit; however, these are not available in much of the world. <br>

# Attribute Information <br>

1) gender: "Male", "Female" or "Other" <br>
2) age: age of the patient <br>
3) hypertension: 0 if the patient doesn't have hypertension, 1 if the patient has hypertension <br>
4) heart_disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease <br>
5) ever_married: "No" or "Yes" <br>
6) work_type: "children", "Govt_jov", "Never_worked", "Private" or "Self-employed" <br>
7) Residence_type: "Rural" or "Urban" <br>
8) avg_glucose_level: average glucose level in blood <br>
9) bmi: body mass index <br>
10) smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"* <br>
11) stroke: 1 if the patient had a stroke or 0 if not <br>

*Note: "Unknown" in smoking_status means that the information is unavailable for this patient <br>


