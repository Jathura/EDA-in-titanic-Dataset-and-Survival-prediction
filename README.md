
# Titanic Survival Prediction – EDA & Logistic Regression



📌 Project Overview
This project explores the famous Titanic dataset through Exploratory Data Analysis (EDA) and builds a Logistic Regression model to predict passenger survival.
While the Titanic dataset is traditionally used for classification tasks, here we also focus on understanding the data deeply through visualization and preprocessing before building the model.


## Acknowledgements

 - [Titanic Test Dataset](https://www.kaggle.com/competitions/titanic/data?select=test.csv)
 - [Titanic Train Dataset](https://www.kaggle.com/competitions/titanic/data?select=train.csv)
 - [Kaggle Titanic data set where](https://www.kaggle.com/competitions/titanic/data)


##  Dataset Description

Here I will outline the definitions of the columns in the Titanic dataset. You can find this information under the data tab of the competition page.

a). Survived: 0 = Did not survive, 1 = Survived

b). Pclass: Ticket class where 1 = First class, 2 = Second class, 3 = Third class. This can also be seen as a proxy for socio-economic status.

c). Sex: Male or female

d). Age: Age in years, fractional if less than 1

e). SibSp: Number of siblings or spouses aboard the Titanic

f). Parch: Number of parents or children aboard the Titanic

g). Ticket: Passenger ticket number

h). Fare: Passenger fare

i). Cabin: Cabin number

j). Embarked: Point of embarkation where C = Cherbourg, Q = Queenstown, S = Southampton

# Variable Notes

pclass: A proxy for socio-economic status (SES)
1st = Upper
2nd = Middle
3rd = Lower

age: Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5

sibsp: The dataset defines family relations in this way...
Sibling = brother, sister, stepbrother, stepsister
Spouse = husband, wife (mistresses and fiancés were ignored)

parch: The dataset defines family relations in this way...
Parent = mother, father
Child = daughter, son, stepdaughter, stepson
Some children travelled only with a nanny, therefore parch=0 for them.
## 🛠 Workflow
1. Importing Dependencies

We use the following Python libraries:

pandas – Data loading and manipulation

numpy – Numerical operations

matplotlib & seaborn – Data visualization

scikit-learn – Data preprocessing, model training, and evaluation
## Data Loading & Inspection

Loaded train.csv into a Pandas DataFrame

Displayed dataset shape, info, and first few rows to understand structure

Checked missing values with .isnull().sum()
## Handling Missing Values
 - Cabin: Dropped due to high percentage of missing values

 - Age: Filled missing values with mean age

 - Embarked: Filled missing values with mode (most frequent value)
## Exploratory Data Analysis (EDA)
- Descriptive Statistics: Used .describe() for numerical columns

- Visualization Insights:

  - Sex vs Survival → Females had a significantly higher       survival rate than males

  - Pclass vs Survival → Passengers in higher classes had better survival rates

  - Age Distribution → Most passengers were between 20-40 years old
## Encoding Categorical Variables
- Converted categorical values into numeric form for model compatibility:

  - Sex: male → 0, female → 1

  - Embarked: S → 0, C → 1, Q → 2
## Feature & Target Selection
- Features (X): All relevant passenger details excluding - - - Survived, Name, Ticket, and PassengerId

- Target (y): Survived column
## Train-Test Split
- Used train_test_split to divide data:

  - 80% for training

  - 20% for testing
## Model Training

 - Applied Logistic Regression from scikit-learn

 - Logistic Regression is well-suited for binary classification problems like survival prediction


## Model Evaluation
- Calculated accuracy score for both training and testing sets:

  - Training Accuracy: 80.90%

  - Testing Accuracy: 78.21%
## Key Insights from EDA
- Females had a much higher survival rate than males despite being fewer in number.

- Higher-class passengers (Pclass = 1) were more likely to survive.

- Younger passengers had a slightly higher survival rate.

- Passengers who embarked from Cherbourg (C) had higher chances of survival compared to Southampton (S) and Queenstown (Q).
## Installation

Esential libraries  for EDA

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```
    
## How to run the project
- Clone this repository

- Place train.csv in the working directory

- Open the Jupyter Notebook (https://colab.research.google.com/drive/1CihTsD6gl8pT0oNgLkzJLoMV5eVTnWvJ#scrollTo=EEET7DhkQaHa) or upload to Google Colab

- Run all cells to execute EDA and train the model

- Observe the visualizations and accuracy results
## 🔮 Future Improvements
- Try Random Forest or Gradient Boosting for potentially higher accuracy

- Perform hyperparameter tuning on Logistic Regression

- Use feature scaling to improve model convergence

- Apply cross-validation for more robust performance metrics
# Hi, I'm Nikhil sachan! 👋

Second Year Student At IIT Patna doing BS in Computer Science and Data Analytics
## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://katherineoelsner.com/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nikhilsachan01/)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://x.com/NikhilSach35241)

