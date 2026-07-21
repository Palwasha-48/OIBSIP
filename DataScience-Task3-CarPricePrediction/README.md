# 🚗 Car Price Prediction using Machine Learning

## 📑 Table of Contents

- [� Car Price Prediction using Machine Learning](#-car-price-prediction-using-machine-learning)
  - [📑 Table of Contents](#-table-of-contents)
- [📌 Project Overview](#-project-overview)
- [❓ Problem Statement](#-problem-statement)
- [💡 Solution](#-solution)
- [🤖 What is Machine Learning?](#-what-is-machine-learning)
- [📈 What is Regression?](#-what-is-regression)
    - [Examples of Regression](#examples-of-regression)
- [🔄 Classification vs Regression](#-classification-vs-regression)
- [🚙 About the Dataset](#-about-the-dataset)
- [🎯 Project Goal](#-project-goal)
- [📊 Dataset Information](#-dataset-information)
    - [Dataset Features](#dataset-features)
- [🧹 Data Cleaning](#-data-cleaning)
- [🛠️ Feature Engineering](#️-feature-engineering)
  - [🚗 Car Age](#-car-age)
  - [🏷️ Brand Extraction](#️-brand-extraction)
- [🔍 Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)
- [📈 Data Visualization](#-data-visualization)
- [💰 Selling Price Distribution](#-selling-price-distribution)
    - [Observation](#observation)
- [⛽ Selling Price vs Fuel Type](#-selling-price-vs-fuel-type)
    - [Observation](#observation-1)
- [📅 Selling Price vs Car Age](#-selling-price-vs-car-age)
    - [Observation](#observation-2)
- [🔥 Correlation Heatmap](#-correlation-heatmap)
- [🏷️ Encoding Categorical Variables](#️-encoding-categorical-variables)
- [✂️ Train-Test Split](#️-train-test-split)
    - [Training Set](#training-set)
    - [Testing Set](#testing-set)
- [🤖 Machine Learning Models](#-machine-learning-models)
- [📈 Linear Regression](#-linear-regression)
    - [Advantages](#advantages)
- [🌲 Random Forest Regressor](#-random-forest-regressor)
    - [Advantages](#advantages-1)
- [⚖️ Why Compare Multiple Models?](#️-why-compare-multiple-models)
- [📉 Model Evaluation](#-model-evaluation)
- [📏 Mean Absolute Error (MAE)](#-mean-absolute-error-mae)
- [📐 Root Mean Squared Error (RMSE)](#-root-mean-squared-error-rmse)
- [🎯 R² Score (Coefficient of Determination)](#-r-score-coefficient-of-determination)
- [🏆 Model Comparison](#-model-comparison)
- [📊 Feature Importance](#-feature-importance)
- [📈 Results](#-results)
- [💡 Key Learnings](#-key-learnings)
- [📂 Project Structure](#-project-structure)
- [⚙️ Technologies Used](#️-technologies-used)
- [🚀 How to Run the Project](#-how-to-run-the-project)
    - [Step 1](#step-1)
    - [Step 2](#step-2)
    - [Step 3](#step-3)
    - [Step 4](#step-4)
- [📊 Project Outputs](#-project-outputs)
- [🌍 Real-World Applications](#-real-world-applications)
- [🔮 Future Improvements](#-future-improvements)
- [🎯 What I Learned](#-what-i-learned)
- [🙏 Acknowledgements](#-acknowledgements)
- [🙋 About Me](#-about-me)
  - [**Palwasha**](#palwasha)
- [⭐ Support](#-support)


> 🎓 Oasis Infobyte Data Science Internship – Task 3

This project focuses on predicting the **selling price of a used car** using Machine Learning. Instead of guessing a car's value manually, the model learns from historical car data and predicts an estimated selling price based on different features.

---

# 📌 Project Overview

The price of a used car depends on many factors such as its brand, age, fuel type, transmission, kilometers driven, and ownership history.

Manually estimating the price of every used car can be difficult and may lead to inaccurate pricing.

In this project, I built a **Machine Learning Regression Model** that predicts the selling price of a used car by learning patterns from historical data.

This project helped me understand the complete Machine Learning workflow, including data cleaning, feature engineering, exploratory data analysis (EDA), model training, evaluation, and comparison of different regression models.

---

# ❓ Problem Statement

Suppose you want to buy or sell a used car.

A common question is:

> **"What should be the fair selling price of this car?"**

The answer depends on several factors, such as:

- 🚗 Brand
- 📅 Manufacturing Year
- ⛽ Fuel Type
- ⚙️ Transmission
- 🛣️ Kilometers Driven
- 👤 Number of Previous Owners

Instead of estimating the price manually, this project uses Machine Learning to predict the selling price based on these features.

---

# 💡 Solution

To solve this problem, I developed a Machine Learning Regression model.

The complete workflow included:

- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Data Visualization
- Encoding Categorical Features
- Feature Correlation Analysis
- Train-Test Split
- Training Multiple Regression Models
- Model Evaluation
- Model Comparison

Finally, the best-performing model was selected based on its evaluation metrics.

---

# 🤖 What is Machine Learning?

Machine Learning is a branch of Artificial Intelligence that enables computers to learn patterns from data and make predictions without being explicitly programmed.

Instead of creating hundreds of manual rules, we provide historical data to the model.

The model studies the relationship between the input features and the output, then uses that knowledge to make predictions for new data.

---

# 📈 What is Regression?

Regression is a type of Machine Learning used when the output is a **continuous numerical value**.

Unlike Classification, which predicts categories, Regression predicts actual numbers.

### Examples of Regression

- Predicting House Prices
- Predicting Car Prices
- Predicting Salary
- Predicting Sales Revenue
- Predicting Stock Prices

This project is a **Regression Problem** because the model predicts the selling price of a used car.

---

# 🔄 Classification vs Regression

| Classification | Regression |
|---------------|------------|
| Predicts Categories | Predicts Numerical Values |
| Example: Spam or Not Spam | Example: Car Price |
| Example: Iris Flower Species | Example: House Price |
| Output = Labels | Output = Numbers |

While my previous Iris Flower Classification project predicted the **type of flower**, this project predicts the **selling price of a car**.

---

# 🚙 About the Dataset

This project uses the **CarDekho Vehicle Dataset**, which contains information about used cars and their selling prices.

Each row in the dataset represents one car with different attributes that influence its market value.

The dataset includes features such as:

- Car Name
- Manufacturing Year
- Selling Price
- Present Price
- Kilometers Driven
- Fuel Type
- Seller Type
- Transmission
- Owner

These features help the Machine Learning models learn the relationship between a car's characteristics and its selling price.

---

# 🎯 Project Goal

The main objective of this project is to train a Machine Learning model that can accurately predict the selling price of a used car.

By learning from historical car data, the model can estimate the price of a new car record that it has never seen before.

Such prediction systems are useful for:

- 🚗 Car Buyers
- 🚗 Car Sellers
- 🚗 Dealerships
- 🚗 Online Car Marketplaces

They help users estimate a fair market price before buying or selling a vehicle.

---

---

# 📊 Dataset Information

The CarDekho dataset contains information about used cars along with their selling prices and other important details.

Each row represents a single car, while each column describes one of its characteristics.

The dataset includes both **numerical** and **categorical** features, making it suitable for practicing data preprocessing, feature engineering, visualization, and regression modeling.

### Dataset Features

| Feature | Description |
|----------|-------------|
| Car_Name | Name of the car |
| Year | Manufacturing year |
| Selling_Price | Selling price of the car (Target Variable) |
| Present_Price | Current ex-showroom price |
| Kms_Driven | Total kilometers driven |
| Fuel_Type | Petrol, Diesel, or CNG |
| Seller_Type | Dealer or Individual |
| Transmission | Manual or Automatic |
| Owner | Number of previous owners |

---

# 🧹 Data Cleaning

Real-world datasets often contain missing values, duplicate records, or inconsistent data.

Before training any Machine Learning model, it is important to clean the dataset.

During this project, I performed several preprocessing steps to improve data quality.

These included:

- Checking for missing values
- Removing duplicate records
- Inspecting data types
- Standardizing categorical values where necessary

Cleaning the dataset helps the model learn from accurate and consistent information.

---

# 🛠️ Feature Engineering

Feature Engineering is the process of creating new features from existing data to improve model performance.

In this project, two new features were created.

## 🚗 Car Age

The original dataset contained the manufacturing year of each car.

Instead of using the year directly, I calculated the **Car Age**.

```python
Car Age = Current Year - Manufacturing Year
```

This feature is more meaningful because buyers usually think in terms of **how old a car is**, not the year it was manufactured.

---

## 🏷️ Brand Extraction

The `Car_Name` column contained both the brand and the model name.

For example:

```
Maruti Swift
Honda City
Hyundai i20
Toyota Corolla
```

Only the **brand name** was extracted from the car name.

This helped reduce unnecessary information while preserving an important feature that influences the selling price.

---

# 🔍 Exploratory Data Analysis (EDA)

Before training any Machine Learning model, it is important to understand the data.

This process is called **Exploratory Data Analysis (EDA).**

EDA helps answer questions such as:

- Which features affect the selling price the most?
- Are there any unusual values?
- How is the selling price distributed?
- Which variables are strongly related?

By understanding these patterns first, better modeling decisions can be made later.

---

# 📈 Data Visualization

Several visualizations were created to better understand the dataset.

These included:

- Distribution Plot
- Box Plot
- Scatter Plot
- Correlation Heatmap

Each visualization revealed useful insights about the data.

---

# 💰 Selling Price Distribution

The distribution plot was used to understand how car prices are spread across the dataset.

### Observation

- Most used cars have relatively lower selling prices.
- Only a small number of cars have very high selling prices.
- The data is positively skewed because expensive cars are less common.

Understanding the target variable helps in selecting suitable regression models.

---

# ⛽ Selling Price vs Fuel Type

A box plot was created to compare selling prices across different fuel types.

### Observation

The visualization showed that the selling price varies depending on the fuel type.

This indicates that fuel type can influence a car's market value and should be considered during model training.

---

# 📅 Selling Price vs Car Age

A scatter plot was created to study the relationship between car age and selling price.

### Observation

A general downward trend can be observed.

As the age of a car increases, its selling price usually decreases.

This relationship makes **Car Age** an important feature for predicting prices.

---

# 🔥 Correlation Heatmap

A correlation heatmap was used to measure the relationship between numerical variables.

Correlation values range from **-1 to +1**.

- **+1** → Strong Positive Correlation
- **0** → No Correlation
- **-1** → Strong Negative Correlation

The heatmap helped identify which numerical features had the strongest relationship with the selling price.

This analysis also helped understand which variables contributed most to the prediction.

---

# 🏷️ Encoding Categorical Variables

Machine Learning models work with numerical values rather than text.

Therefore, categorical features such as:

- Fuel Type
- Seller Type
- Transmission
- Brand

were converted into numerical format using encoding techniques.

This allowed the regression models to process categorical information effectively.

---

# ✂️ Train-Test Split

To evaluate the model fairly, the dataset was divided into two parts.

### Training Set

The model learns patterns from this data.

### Testing Set

The model is evaluated using unseen data to measure how well it generalizes.

In this project, the dataset was split into:

- **80% Training Data**
- **20% Testing Data**

This helps reduce overfitting and provides a more reliable evaluation of model performance.

---

---

# 🤖 Machine Learning Models

To predict the selling price of used cars, I trained and compared multiple Machine Learning regression models.

Instead of relying on a single algorithm, comparing different models helps identify which one performs best for this dataset.

The models used in this project include:

- Linear Regression
- Random Forest Regressor

By comparing their performance, I was able to understand the strengths and limitations of each model.

---

# 📈 Linear Regression

Linear Regression is one of the simplest and most widely used regression algorithms.

It predicts the relationship between the input features and the target variable by fitting a straight line through the data.

The model assumes that changes in the input features have a linear relationship with the selling price.

### Advantages

- Simple and easy to understand
- Fast training
- Easy to interpret
- Works well when relationships are approximately linear

However, real-world car prices often depend on complex relationships, which can limit the performance of Linear Regression.

---

# 🌲 Random Forest Regressor

Random Forest is an ensemble Machine Learning algorithm.

Instead of relying on a single decision tree, it builds many decision trees and combines their predictions.

The final prediction is calculated by averaging the outputs of all trees.

### Advantages

- Handles complex relationships
- Reduces overfitting
- Works well on structured datasets
- Usually provides higher prediction accuracy

Because car prices depend on many different factors, Random Forest often performs better than simpler regression models.

---

# ⚖️ Why Compare Multiple Models?

Every Machine Learning algorithm has its own strengths and weaknesses.

Comparing different models helps answer questions such as:

- Which model predicts more accurately?
- Which model handles the dataset better?
- Which model should be selected for deployment?

Rather than assuming one algorithm is always the best, evaluating multiple models leads to more reliable results.

---

# 📉 Model Evaluation

After training the models, their performance was evaluated using three commonly used regression metrics.

These metrics help measure how close the predicted prices are to the actual selling prices.

---

# 📏 Mean Absolute Error (MAE)

MAE measures the average difference between the predicted price and the actual price.

A lower MAE indicates better performance.

For example, if the MAE is low, it means the model's predictions are generally close to the true selling prices.

---

# 📐 Root Mean Squared Error (RMSE)

RMSE also measures prediction error but gives more importance to larger errors.

This makes RMSE useful when large prediction mistakes should be penalized more heavily.

Lower RMSE values indicate better model performance.

---

# 🎯 R² Score (Coefficient of Determination)

The R² Score measures how well the model explains the variation in the target variable.

Its value ranges from 0 to 1.

- **1** → Perfect prediction
- **0** → No explanatory power

A higher R² Score indicates that the model captures the relationship between the features and the selling price more effectively.

---

# 🏆 Model Comparison

After evaluating all models, their performance was compared using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

The model with:

- Lower MAE
- Lower RMSE
- Higher R² Score

was considered the best-performing model for this dataset.

---

# 📊 Feature Importance

One advantage of tree-based models such as Random Forest is that they can estimate the importance of each feature.

Feature Importance helps answer questions like:

- Which feature affects the selling price the most?
- Which variables contribute the least?

By analyzing feature importance, we gain a better understanding of the factors influencing used car prices.

---

# 📈 Results

The trained models successfully learned the relationship between car features and their selling prices.

The evaluation metrics showed that the selected model was able to make reliable predictions on unseen data.

This demonstrates the effectiveness of Machine Learning in solving real-world price prediction problems.

---

# 💡 Key Learnings

Through this project, I learned how to:

- Clean and preprocess real-world datasets.
- Perform feature engineering.
- Explore data using EDA.
- Train multiple regression models.
- Evaluate models using MAE, RMSE, and R² Score.
- Compare different algorithms based on performance.
- Interpret feature importance instead of relying only on prediction accuracy.

Overall, this project strengthened my understanding of Regression and its practical applications in Data Science.

---

---

# 📂 Project Structure

```
Car-Price-Prediction/
│
├── Car_Price_Prediction.ipynb
├── car data.csv
├── README.md
├── requirements.txt
│
├── images/
│   ├── price_distribution.png
│   ├── fuel_type_boxplot.png
│   ├── car_age_scatter.png
│   ├── heatmap.png
│   └── feature_importance.png
│
└── LICENSE
```

This project is organized in a simple and structured way, making it easy to understand and reproduce.

---

# ⚙️ Technologies Used

The following tools and libraries were used in this project:

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| Pandas | Data Manipulation |
| NumPy | Numerical Operations |
| Matplotlib | Data Visualization |
| Seaborn | Exploratory Data Analysis |
| Scikit-learn | Machine Learning |
| Jupyter Notebook | Development Environment |

---

# 🚀 How to Run the Project

### Step 1

Clone this repository.

```bash
git clone https://github.com/Palwasha-48/OIBSIP.git
```

---

### Step 2

Open the project folder.

```bash
cd OIBSIP
```

---

### Step 3

Install the required libraries.

```bash
pip install -r requirements.txt
```

---

### Step 4

Launch Jupyter Notebook.

```bash
jupyter notebook
```

Open the notebook and run all cells to reproduce the complete analysis and predictions.

---

# 📊 Project Outputs

This project includes several visualizations that help understand the dataset and model performance.

Some of the outputs include:

- Selling Price Distribution
- Selling Price vs Fuel Type
- Selling Price vs Car Age
- Correlation Heatmap
- Feature Importance Chart
- Model Evaluation Results

> 📌 You can save these graphs inside the `images` folder and display them here later if you want.

---

# 🌍 Real-World Applications

Car Price Prediction systems are widely used in the automobile industry.

Some real-world applications include:

- 🚗 Online Used Car Marketplaces
- 🏢 Car Dealerships
- 💰 Vehicle Loan & Insurance Companies
- 📈 Car Valuation Platforms
- 📱 Automobile Mobile Applications

Such systems help buyers and sellers estimate a fair market price quickly and reduce manual guesswork.

---

# 🔮 Future Improvements

This project can be enhanced in several ways:

- Train additional regression models such as XGBoost or Gradient Boosting.
- Perform Hyperparameter Tuning.
- Apply Cross Validation for more reliable evaluation.
- Build a Streamlit web application for real-time predictions.
- Deploy the model online for public use.
- Train the model using a larger and more diverse dataset.

---

# 🎯 What I Learned

This project helped me understand that predicting a continuous value is different from classifying categories.

Through this project, I learned how to:

- Clean and preprocess real-world datasets.
- Create meaningful features using Feature Engineering.
- Explore datasets through EDA and visualizations.
- Train and compare multiple Regression models.
- Evaluate models using MAE, RMSE, and R² Score.
- Interpret Feature Importance.
- Understand how Machine Learning can solve practical business problems.

Overall, this project strengthened my understanding of Regression and increased my confidence in building Machine Learning models.

---

# 🙏 Acknowledgements

This project was completed as part of the **Oasis Infobyte Data Science Internship**.

I sincerely thank Oasis Infobyte for providing practical projects that helped me apply Machine Learning concepts to solve real-world problems.

---

# 🙋 About Me

## **Palwasha**

**Data Science Student | Machine Learning Learner | Frontend Developer**

**GitHub:**  
https://github.com/Palwasha-48

**LinkedIn:**  
https://linkedin.com/in/palwasheyqureshi/

---

# ⭐ Support

If you found this project helpful, consider giving this repository a ⭐.

Your support motivates me to continue learning, building, and sharing more Data Science and Machine Learning projects.

Thank you for visiting my repository! 💙
