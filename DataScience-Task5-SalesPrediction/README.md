# 📺 Sales Prediction using Machine Learning

> 🎓 Oasis Infobyte Data Science Internship – Task 5

This project focuses on predicting **product sales** using Machine Learning based on advertising spending across different media channels.

Businesses spend money on advertisements through **TV, Radio, and Newspaper**, but an important question is:

> **"How much sales can we expect from this advertising budget?"**

Instead of making guesses, this project uses Machine Learning to learn from historical advertising data and predict future sales.

---

# 📑 Table of Contents

- [📺 Sales Prediction using Machine Learning](#-sales-prediction-using-machine-learning)
- [📑 Table of Contents](#-table-of-contents)
- [📌 Project Overview](#-project-overview)
- [❓ Problem Statement](#-problem-statement)
- [💡 Solution](#-solution)
- [🤖 What is Machine Learning?](#-what-is-machine-learning)
- [📈 What is Regression?](#-what-is-regression)
    - [Examples of Regression](#examples-of-regression)
- [📺 About the Advertising Dataset](#-about-the-advertising-dataset)
- [🎯 Project Goal](#-project-goal)
- [📊 Dataset Information](#-dataset-information)
- [🧹 Data Cleaning](#-data-cleaning)
- [🔍 Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)
- [📈 Data Visualization](#-data-visualization)
- [📺 TV Advertising vs Sales](#-tv-advertising-vs-sales)
    - [Observation](#observation)
- [📻 Radio Advertising vs Sales](#-radio-advertising-vs-sales)
    - [Observation](#observation-1)
- [📰 Newspaper Advertising vs Sales](#-newspaper-advertising-vs-sales)
    - [Observation](#observation-2)
- [🔥 Correlation Analysis](#-correlation-analysis)
- [✂️ Train-Test Split](#️-train-test-split)
    - [Training Set](#training-set)
    - [Testing Set](#testing-set)
  - [This approach helps evaluate the model on data it has not seen before.](#this-approach-helps-evaluate-the-model-on-data-it-has-not-seen-before)
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
- [📊 Residual Plot](#-residual-plot)
    - [Observation](#observation-3)
- [🏆 Model Comparison](#-model-comparison)
- [🎯 Results](#-results)
- [💡 Key Learnings](#-key-learnings)
  - [Overall, this project strengthened my understanding of Regression and its practical applications in Sales Prediction.](#overall-this-project-strengthened-my-understanding-of-regression-and-its-practical-applications-in-sales-prediction)
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

---

# 📌 Project Overview

Advertising plays an important role in increasing product sales.

However, companies often spend large amounts of money on advertisements without knowing how much sales those campaigns will generate.

In this project, I built a **Machine Learning Regression Model** that predicts product sales using advertising budgets spent on **TV, Radio, and Newspaper**.

The project follows the complete Machine Learning workflow, including data preprocessing, exploratory data analysis (EDA), visualization, model training, evaluation, and prediction.

---

# ❓ Problem Statement

Every business wants to know whether its advertising budget is being used effectively.

For example:

- Will increasing the TV advertising budget improve sales?
- Does Radio advertising have a strong impact on sales?
- Is Newspaper advertising still effective?

Finding these answers manually can be difficult.

This project uses Machine Learning to analyze historical advertising data and predict product sales based on advertising spending.

---

# 💡 Solution

To solve this problem, I developed a Machine Learning Regression model.

The complete workflow included:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Data Visualization
- Correlation Analysis
- Train-Test Split
- Training Multiple Regression Models
- Model Evaluation
- Model Comparison

Finally, the best-performing model was selected based on its evaluation metrics.

---

# 🤖 What is Machine Learning?

Machine Learning is a branch of Artificial Intelligence that enables computers to learn patterns from data and make predictions without being explicitly programmed.

Instead of writing manual rules, we provide historical data to the model.

The model learns the relationship between the input features and the target value, then uses that knowledge to make predictions for new data.

---

# 📈 What is Regression?

Regression is a type of Machine Learning used to predict **continuous numerical values**.

Unlike Classification, which predicts categories, Regression predicts actual numbers.

### Examples of Regression

- Predicting Product Sales
- Predicting House Prices
- Predicting Car Prices
- Predicting Stock Prices
- Predicting Monthly Revenue

This project is a **Regression Problem** because the model predicts the **sales value**.

---

# 📺 About the Advertising Dataset

This project uses the **Advertising Dataset**, which contains advertising budgets spent on different media channels along with product sales.

The dataset includes spending on:

- 📺 TV Advertising
- 📻 Radio Advertising
- 📰 Newspaper Advertising

The target variable is **Sales**.

The Machine Learning model learns how advertising spending influences sales and uses this relationship to predict future sales.

---

# 🎯 Project Goal

The main objective of this project is to build a Machine Learning model that can accurately predict product sales using advertising data.

Such prediction systems help businesses:

- Make smarter marketing decisions
- Estimate future sales
- Optimize advertising budgets
- Improve business planning
- Reduce unnecessary advertising expenses

By learning from historical data, the model can estimate sales for new advertising budgets that it has never seen before.

---

# 📊 Dataset Information

The Advertising dataset contains information about advertising budgets and product sales.

Each row represents one advertising campaign, while each column describes the amount spent on different advertising channels.

The dataset consists of the following features:

| Feature | Description |
|----------|-------------|
| TV | Advertising budget spent on TV |
| Radio | Advertising budget spent on Radio |
| Newspaper | Advertising budget spent on Newspapers |
| Sales | Product sales (Target Variable) |

The objective is to predict **Sales** using the advertising budgets.

---

# 🧹 Data Cleaning

Before training the Machine Learning models, the dataset was inspected to ensure that it was ready for analysis.

The following preprocessing steps were performed:

- Loaded the dataset using Pandas.
- Checked the dataset shape.
- Displayed the first few rows.
- Reviewed data types and summary statistics.

The dataset was already clean and did not require major preprocessing.

---

# 🔍 Exploratory Data Analysis (EDA)

Exploratory Data Analysis (EDA) was performed to understand the dataset before training the models.

EDA helps identify relationships between variables and provides useful insights through visualizations.

This project includes:

- Pair Plot
- Scatter Plots
- Correlation Heatmap

These visualizations helped understand how advertising spending influences product sales.

---

# 📈 Data Visualization

Several visualizations were created to explore the relationship between advertising budgets and sales.

The following plots were used:

- Pair Plot
- TV vs Sales Scatter Plot
- Radio vs Sales Scatter Plot
- Newspaper vs Sales Scatter Plot
- Correlation Heatmap

These graphs helped identify trends and relationships in the dataset.

---

# 📺 TV Advertising vs Sales

A scatter plot was created to analyze the relationship between TV advertising and product sales.

### Observation

The plot shows a strong positive relationship between TV advertising spending and sales.

In general, higher TV advertising budgets are associated with higher product sales.

---

# 📻 Radio Advertising vs Sales

A scatter plot was created to study the relationship between Radio advertising and sales.

### Observation

Radio advertising also shows a positive relationship with sales, although the trend is slightly weaker than TV advertising.

This indicates that Radio advertising contributes to improving product sales.

---

# 📰 Newspaper Advertising vs Sales

A scatter plot was created to examine the effect of Newspaper advertising on sales.

### Observation

Compared to TV and Radio, Newspaper advertising shows a much weaker relationship with sales.

This suggests that Newspaper advertising has a smaller influence on product sales in this dataset.

---

# 🔥 Correlation Analysis

A correlation heatmap was used to measure the relationship between numerical variables.

Correlation values range from **-1 to +1**.

- **+1** → Strong Positive Correlation
- **0** → No Correlation
- **-1** → Strong Negative Correlation

The heatmap helps identify which advertising channel has the strongest relationship with product sales.

---

# ✂️ Train-Test Split

To evaluate the model fairly, the dataset was divided into two parts.

### Training Set

The model learns patterns from this data.

### Testing Set

The model is evaluated using unseen data to measure how well it predicts new values.

In this project, the dataset was divided into:

- **80% Training Data**
- **20% Testing Data**

This approach helps evaluate the model on data it has not seen before.
---

# 🤖 Machine Learning Models

To predict product sales, I trained and compared two Machine Learning regression models.

Instead of relying on a single algorithm, comparing multiple models helps identify which one performs better on the dataset.

The models used in this project are:

- Linear Regression
- Random Forest Regressor

Each model was trained using the training dataset and evaluated using unseen test data.

---

# 📈 Linear Regression

Linear Regression is one of the most commonly used regression algorithms.

It learns the relationship between advertising budgets and product sales by fitting a straight line through the data.

### Advantages

- Simple and easy to understand
- Fast to train
- Easy to interpret
- Works well for linear relationships

Linear Regression serves as a strong baseline model for prediction tasks.

---

# 🌲 Random Forest Regressor

Random Forest is an ensemble learning algorithm that combines multiple decision trees.

Instead of relying on a single tree, it averages the predictions of many trees to improve accuracy and reduce overfitting.

### Advantages

- Handles complex relationships
- Reduces overfitting
- Works well on structured datasets
- Often provides better prediction performance

---

# ⚖️ Why Compare Multiple Models?

Every Machine Learning algorithm has its own strengths and limitations.

Comparing multiple models helps answer questions such as:

- Which model predicts sales more accurately?
- Which model performs better on unseen data?
- Which model should be selected for future predictions?

The comparison was based on evaluation metrics rather than assumptions.

---

# 📉 Model Evaluation

After training the models, their performance was evaluated using three common regression metrics.

These metrics measure how close the predicted sales are to the actual sales values.

---

# 📏 Mean Absolute Error (MAE)

MAE measures the average difference between the predicted sales and the actual sales.

A lower MAE indicates better model performance.

---

# 📐 Root Mean Squared Error (RMSE)

RMSE measures prediction error while giving more importance to larger errors.

Lower RMSE values indicate more accurate predictions.

---

# 🎯 R² Score (Coefficient of Determination)

The R² Score measures how well the model explains the variation in the target variable.

Its value ranges from **0 to 1**.

- **1** → Perfect prediction
- **0** → No explanatory power

A higher R² Score indicates better model performance.

---

# 📊 Residual Plot

A residual plot was used to evaluate the prediction errors of the regression model.

Residuals represent the difference between the actual sales and the predicted sales.

### Observation

If the residuals are randomly scattered around zero, it indicates that the model has learned the data well and does not show obvious prediction patterns.

---

# 🏆 Model Comparison

Both models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

The model with lower error values and a higher R² Score was considered the better-performing model.

---

# 🎯 Results

The trained models successfully learned the relationship between advertising spending and product sales.

The evaluation results showed that Machine Learning can effectively predict sales using historical advertising data.

This demonstrates how data-driven approaches can support smarter marketing decisions.

---

# 💡 Key Learnings

Through this project, I learned how to:

- Understand advertising datasets using EDA.
- Visualize relationships between advertising channels and sales.
- Train multiple regression models.
- Evaluate models using MAE, RMSE, and R² Score.
- Compare different algorithms based on their performance.
- Understand how Machine Learning can help businesses make data-driven decisions.

Overall, this project strengthened my understanding of Regression and its practical applications in Sales Prediction.
---

# 📂 Project Structure

```
Sales-Prediction/
│
├── task5.ipynb
├── Advertising.csv
├── README.md
├── requirements.txt
│
├── images/
│   ├── pairplot.png
│   ├── tv_vs_sales.png
│   ├── radio_vs_sales.png
│   ├── newspaper_vs_sales.png
│   ├── correlation_heatmap.png
│   └── residual_plot.png
│
└── LICENSE
```

The project is organized in a simple and structured way, making it easy to understand and reproduce.

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

This project includes several visualizations that help understand the relationship between advertising spending and product sales.

Some of the outputs include:

- Pair Plot
- TV vs Sales Scatter Plot
- Radio vs Sales Scatter Plot
- Newspaper vs Sales Scatter Plot
- Correlation Heatmap
- Residual Plot
- Model Evaluation Results

> 📌 You can save these graphs inside the `images` folder and display them here later if you want.

---

# 🌍 Real-World Applications

Sales Prediction models are widely used across different industries.

Some real-world applications include:

- 📈 Marketing Campaign Planning
- 💰 Advertising Budget Optimization
- 🛍️ Retail Sales Forecasting
- 📦 Inventory Management
- 📊 Business Decision Making

These systems help businesses estimate future sales, improve marketing strategies, and allocate advertising budgets more effectively.

---

# 🔮 Future Improvements

This project can be enhanced in several ways:

- Train additional regression models such as XGBoost or Gradient Boosting.
- Perform Hyperparameter Tuning.
- Apply Cross Validation for more reliable evaluation.
- Build a Streamlit web application for real-time sales prediction.
- Deploy the model online for public use.
- Train the model using a larger and more diverse dataset.

---

# 🎯 What I Learned

This project helped me understand how advertising data can be used to predict product sales using Machine Learning.

Through this project, I learned how to:

- Explore datasets using EDA and visualizations.
- Understand relationships between advertising channels and sales.
- Train and compare multiple regression models.
- Evaluate models using MAE, RMSE, and R² Score.
- Interpret residual plots to analyze prediction errors.
- Apply Machine Learning to solve real-world business problems.

Overall, this project strengthened my understanding of Regression and increased my confidence in building predictive Machine Learning models.

---

# 🙏 Acknowledgements

This project was completed as part of the **Oasis Infobyte Data Science Internship**.

I sincerely thank Oasis Infobyte for providing practical projects that helped me apply Machine Learning concepts to solve real-world business problems.

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