# Titanic_Survival_Predication
This project involves analyzing the Titanic dataset to predict survival outcomes by training a Logistic Regression model, evaluating its performance using accuracy and confusion matrix, and visualizing results.

**Dataset**

The dataset used includes the following columns:

    • PassengerId: Unique ID for each passenger  
    • Survived: Survival status (0 = No, 1 = Yes)  
    • Pclass: Passenger class (1, 2, 3)  
    • Name: Name of the passenger  
    • Sex: Gender of the passenger  
    • Age: Age of the passenger  
    • SibSp: Number of siblings or spouses aboard  
    • Parch: Number of parents or children aboard  
    • Ticket: Ticket number  
    • Fare: Fare paid for the ticket  
    • Cabin: Cabin number  
    • Embarked: Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)  

**Analysis and Data Wrangling**

   • Loading Data:
          The dataset is loaded into a Pandas DataFrame.
  
   • Initial Exploration:
          Count plots, Histograms and Violin plots are used for data visualization.
  
   • Data Cleaning:
          Missing values in Age columns are replaced with the mean of the ages.
          The Cabin column is dropped due to its high proportion of missing values.
          Rows with duplicate values are removed.
          Categorical variables (Sex, Embarked) are converted into dummy variables.
  
    • Feature Selection:
          Unnecessary columns are neglected.
          The dataset is prepared for model training by splitting it into feature variables (X) and target variable (y).
  
    • Model Training:
          Logistic Regression is used to train the model.
          The dataset is split into training and testing sets.
  
    • Evaluation:
          Classification report, confusion matrix, and accuracy score are used to evaluate model performance.
        
**Results**

The Logistic Regression model achieved an accuracy score of approximately 0.785. Detailed metrics including classification report and confusion matrix provide further insights into model performance.

         precision    recall  f1-score   support  

   0       0.80      0.85      0.82        110  
   1       0.74      0.65      0.69        69  

accuracy 0.7765

**Confusion Matrix**

[[94 16] [24 45]]

**Conclusion**

The logistic regression model achieved an accuracy of 77.65% in predicting Titanic survival outcomes. This indicates the model effectively distinguishes between survivors and non-survivors based on key features such as Pclass, Age, Sex, Fare, and Embarked. With Key Features:

    • Model Performance: The model shows good predictive power with balanced precision and recall.
    • Feature Importance: Key features significantly impact accuracy, while handling missing data was crucial.
    • Future Improvements: Further enhancements could include exploring more advanced models or additional feature engineering.
