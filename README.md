 
# heart-disease-classification

To work on this Project Download Miniconda3 Into your system

Open miniconda3 prompt shell and download **pandas, numpy, matplotlib, scikit learn** packages using following command :

` conda install pandas numpy matplotlib scikit-learn`

## The clear working of this project is briefly worked in Jupyter Notebook (Attached with this repository). Every step explanation is explained with markdowns in Jupyter Notebook.

## Let's see outlook of this project :

**This project looks into using various Python-based machine learning and data science libraries in an attempt to build a machine learning model capable of predicting whether or not someone has heart disease based on their medical attributes.**

## We're going to take the following approach :

1. Problem definition
2. Data
3. Evaluation
4. Features
5. Modelling
6. Experimentation

## Data set

The original dataset used in this project came from the Cleavland data from the UCI Macine Learning Repository. https://archive.ics.uci.edu/dataset/45/heart+disease

### Data Set Column Parameters :

1. age: Displays the age of the individual.

2. sex: Displays the gender of the individual using the following format :
    * 1 = male
    * 0 = female

3. cp- Chest-pain type: displays the type of chest-pain experienced by the individual using the following format :
      * 0 = typical angina
      * 1 = atypical angina
      * 2 = non — anginal pain
      * 3 = asymptotic

4. trestbps- Resting Blood Pressure: displays the resting blood pressure value of an individual in mmHg (unit). anything above 130-140 is typically cause for concern.

5. chol- Serum Cholestrol: displays the serum cholesterol in mg/dl (unit)

6. fbs- Fasting Blood Sugar: compares the fasting blood sugar value of an individual with 120mg/dl.
    * If fasting blood sugar > 120mg/dl then : 1 (true)
    * else : 0 (false) '>126' mg/dL signals diabetes

7. restecg- Resting ECG : displays resting electrocardiographic results
      * 0 = normal
      * 1 = having ST-T wave abnormality
      * 2 = left ventricular hyperthrophy

8. thalach- Max heart rate achieved : displays the max heart rate achieved by an individual.

9. exang- Exercise induced angina :
      * 1 = yes
      * 0 = no

10. oldpeak- ST depression induced by exercise relative to rest: displays the value which is an integer or float.

11. slope- Slope of the peak exercise ST segment :
       * 0 = upsloping: better heart rate with excercise (uncommon)
       * 1 = flat: minimal change (typical healthy heart)
       * 2 = downsloping: signs of unhealthy heart

12. ca- Number of major vessels (0–3) colored by flourosopy : displays the value as integer or float.

13. thal : Displays the thalassemia :
       * 1,3 = normal
       * 6 = fixed defect
       * 7 = reversible defect: no proper blood movement when excercising

14. target : Displays whether the individual is suffering from heart disease or not :
       * 1 = yes
       * 0 = no


## We're going to try 3 different machine learning models:

1. Logistic Regression
2. K-Nearest Neighbours Classifier
3. Random Forest Classifier

# Screenshots of this project :

## 1. Importing all the required packages and models :

![10](https://github.com/aswin98855/heart-disease-classification/assets/116991167/51c4e24d-331b-462d-ac42-9086da16b2ec)

## 2. Trying different models for our dataset : 

![9](https://github.com/aswin98855/heart-disease-classification/assets/116991167/64e6ed18-7da7-41d5-be67-876fd75267b2)

## 3. Hyperparameter tuning by hand :

![8](https://github.com/aswin98855/heart-disease-classification/assets/116991167/eafa525b-8892-4444-967c-ef4a6d51ba74)

## 4. Graph of Train and Test scores of K-Nearest Neighbours Classifier :

![7](https://github.com/aswin98855/heart-disease-classification/assets/116991167/8c4f76c4-7aa7-40a9-9da0-bf299d63c5aa)

## 5. Hyperparameter tuning with RandomisedSearchCV :

![6](https://github.com/aswin98855/heart-disease-classification/assets/116991167/5d47e4dc-f28d-4577-9989-18b43e11a48b)

## 6. Best params Using Logistic Regression and RandomisedSearchCV with Random Forest Classifier :

![5](https://github.com/aswin98855/heart-disease-classification/assets/116991167/e39126ab-10c2-4791-b20d-0a4aa6161d88)

## 7. Hyperparameter tuning with GridSearchCV :

![4](https://github.com/aswin98855/heart-disease-classification/assets/116991167/0a236d0b-8a34-4f85-a282-74a0ad95ff3f)

## 8. Confusion Matrix using Seaborn's Heatmap : (y_preds values from the Logistic Regression)

![3](https://github.com/aswin98855/heart-disease-classification/assets/116991167/b5202e93-5770-4cb2-bdcb-dc24b8f823ec)

## 9. Cross-validated classification metrics of Logistic Regression with best parameters :

![2](https://github.com/aswin98855/heart-disease-classification/assets/116991167/b32bf0d6-a10f-46d8-ac0d-b69584f88845)

## 10. Feature Importance with Logistic Regression model :

![1](https://github.com/aswin98855/heart-disease-classification/assets/116991167/b8a410b6-03a9-484f-9d70-c4780649a8b2)

## 11. Correlation matrix for dataset :

![11](https://github.com/aswin98855/heart-disease-classification/assets/116991167/8a1fdeeb-be78-4e81-a8c3-f84f11ea3ef8)
 
## 12. ROC (Receiver Operating Characteristic) curve for Logistic Regression :

![12](https://github.com/aswin98855/heart-disease-classification/assets/116991167/9eca0286-711d-41c1-80d1-97aa1354b25e)


### The final accuracy(highest accuracy) after hyper tuning is `0.8852459016393442` with `LogisticRegression()`.
