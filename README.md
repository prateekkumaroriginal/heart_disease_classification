# Predicting heart disease or not, using ML


1. Problem definition
2. Data
3. Evaluation
4. Features
5. Modelling
6. Experimentation

## 1. Problem definition
Given clinical parameters about a patient, predict whether they have heart disease or not.

## 2. Data
The original data came from the Cleavland data from the UCI Machine Learning Repository. https://archive.ics.uci.edu/ml/datasets/heart+Disease

There is also a version of it available on Kaggle. https://www.kaggle.com/datasets/sumaiyatasmeem/heart-disease-classification-dataset

## 3. Evaluation
If we can reach 95% accuracy at predicting whether or not a patient has heart disease during the proof of concept, we'll pursue the project.

## 4. Features
This is where you'll get different information about each of the features in your data. You can do this via doing your own research (such as looking at the links above) or by talking to a subject matter expert (someone who knows about the dataset).

Create data dictionary

1. **age:** Age in years
2. **sex:** Gender (1 = male; 0 = female)
3. **cp:** Chest pain type
   - 0: Typical angina - Chest pain related to a decrease in blood supply to the heart
   - 1: Atypical angina - Chest pain not related to the heart
   - 2: Non-anginal pain - Typically esophageal spasms (non-heart-related)
   - 3: Asymptomatic - Chest pain not showing signs of disease
4. **trestbps:** Resting blood pressure (in mm Hg on admission to the hospital). Anything above 130-140 is typically a cause for concern.
5. **chol:** Serum cholesterol in mg/dL. Serum = LDL + HDL + 0.2 * triglycerides. Above 200 is a cause for concern.
6. **fbs:** Fasting blood sugar > 120 mg/dL (1 = true; 0 = false). '>126' mg/dL signals diabetes.
7. **restecg:** Resting electrocardiographic results
   - 0: Nothing to note
   - 1: ST-T Wave abnormality - Can range from mild symptoms to severe problems, signals non-normal heart beat
   - 2: Possible or definite left ventricular hypertrophy - Enlarged heart's main pumping chamber
8. **thalach:** Maximum heart rate achieved
9. **exang:** Exercise-induced angina (1 = yes; 0 = no)
10. **oldpeak:** ST depression induced by exercise relative to rest. Looks at stress of heart during exercise. An unhealthy heart will stress more.
11. **slope:** The slope of the peak exercise ST segment
    - 0: Upsloping - Better heart rate with exercise (uncommon)
    - 1: Flatsloping - Minimal change (typical healthy heart)
    - 2: Downsloping - Signs of an unhealthy heart
12. **ca:** Number of major vessels (0-3) colored by fluoroscopy. Colored vessels mean the doctor can see the blood passing through. The more blood movement, the better (no clots).
13. **thal:** Thallium stress result
    - 1, 3: Normal
    - 6: Fixed defect - Used to be a defect but okay now
    - 7: Reversible defect - No proper blood movement when exercising
14. **target:** Have disease or not (1 = yes, 0 = no) (= the predicted attribute)
