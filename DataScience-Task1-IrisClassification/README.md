# 🌸 Iris Flower Classification using Machine Learning

## 📑 Table of Contents

- [🌸 Iris Flower Classification using Machine Learning](#-iris-flower-classification-using-machine-learning)
  - [📑 Table of Contents](#-table-of-contents)
- [📌 Project Overview](#-project-overview)
- [❓ Problem Statement](#-problem-statement)
- [💡 Solution](#-solution)
- [🤖 What is Machine Learning?](#-what-is-machine-learning)
- [🎯 What is Classification?](#-what-is-classification)
- [🌼 What is the Iris Dataset?](#-what-is-the-iris-dataset)
- [🌸 Iris Species](#-iris-species)
  - [🌸 Iris Setosa](#-iris-setosa)
  - [🌺 Iris Versicolor](#-iris-versicolor)
  - [🌼 Iris Virginica](#-iris-virginica)
- [🌿 What are Sepals and Petals?](#-what-are-sepals-and-petals)
  - [🌿 Sepal](#-sepal)
  - [🌺 Petal](#-petal)
- [🧠 Why is this Project Important?](#-why-is-this-project-important)
- [📊 Dataset Information](#-dataset-information)
    - [Dataset Summary](#dataset-summary)
- [🔍 Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)
- [📈 Data Visualization](#-data-visualization)
- [🌸 Pair Plot Analysis](#-pair-plot-analysis)
    - [What I observed](#what-i-observed)
    - [Why is this important?](#why-is-this-important)
- [🔥 Correlation Heatmap](#-correlation-heatmap)
- [📦 Feature Selection](#-feature-selection)
- [✂️ Train-Test Split](#️-train-test-split)
    - [Training Data](#training-data)
    - [Testing Data](#testing-data)
- [🤖 Model Training](#-model-training)
- [🔮 Making Predictions](#-making-predictions)
- [🚀 Machine Learning Workflow](#-machine-learning-workflow)
- [🤖 Machine Learning Models](#-machine-learning-models)
- [🧠 Logistic Regression](#-logistic-regression)
    - [Why Logistic Regression?](#why-logistic-regression)
- [👥 K-Nearest Neighbors (KNN)](#-k-nearest-neighbors-knn)
    - [Real-Life Example](#real-life-example)
- [⚖️ Why Compare Multiple Models?](#️-why-compare-multiple-models)
- [📊 Model Performance](#-model-performance)
- [📉 Confusion Matrix](#-confusion-matrix)
- [📋 Classification Report](#-classification-report)
    - [Precision](#precision)
    - [Recall](#recall)
    - [F1-Score](#f1-score)
- [📈 Results](#-results)
    - [Key Findings](#key-findings)
- [💡 Why Did Both Models Achieve 100% Accuracy?](#-why-did-both-models-achieve-100-accuracy)
- [🎯 Key Learnings](#-key-learnings)
- [📂 Project Structure](#-project-structure)
- [⚙️ Technologies Used](#️-technologies-used)
- [🚀 How to Run the Project](#-how-to-run-the-project)
    - [Step 1](#step-1)
    - [Step 2](#step-2)
    - [Step 3](#step-3)
    - [Step 4](#step-4)
- [📸 Project Outputs](#-project-outputs)
- [🌍 Real-World Applications](#-real-world-applications)
- [🔮 Future Improvements](#-future-improvements)
- [🎯 What I Learned](#-what-i-learned)
- [🙏 Acknowledgements](#-acknowledgements)
- [👩‍💻 Author](#-author)
  - [**Palwasha**](#palwasha)
  - [LinkedIn: Palwashey Qureshi](#linkedin-palwashey-qureshi)
- [⭐ Support](#-support)

# 📌 Project Overview

This project was completed as part of my **Data Science Internship at Oasis Infobyte**.

The goal of this project is to build a Machine Learning model that can identify the species of an Iris flower using only its measurements.

Instead of looking at the flower's color or image, the model predicts the species by analyzing four numerical features:

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

Based on these measurements, the model predicts whether the flower belongs to:

- 🌸 Iris Setosa
- 🌺 Iris Versicolor
- 🌼 Iris Virginica

This project helped me understand the complete Machine Learning workflow—from exploring the data to training a model, making predictions, and evaluating its performance.

---

# ❓ Problem Statement

Imagine you discover an Iris flower, but you don't know its species.

Instead of identifying it manually, can a Machine Learning model classify it automatically using only a few measurements?

That is exactly the problem this project solves.

Given:
✔ Sepal Length
✔ Sepal Width
✔ Petal Length
✔ Petal Width

Predict:

➡️ Which Iris species is it?

- Setosa
- Versicolor
- Virginica

---

# 💡 Solution

To solve this problem, I built a supervised Machine Learning classification model.

The complete process included:

- Understanding the dataset
- Exploring the data using EDA
- Finding important features
- Splitting the dataset into training and testing sets
- Training multiple Machine Learning models
- Making predictions
- Evaluating model performance using different metrics

Finally, I compared different models and selected the one that performed best.

---

# 🤖 What is Machine Learning?

Machine Learning (ML) is a branch of Artificial Intelligence that enables computers to learn patterns from data without being explicitly programmed for every situation.

Instead of writing hundreds of rules manually, we provide examples (data), and the model learns those patterns on its own.

For example,

Instead of writing:

"If petal length is greater than 5.5 and petal width is greater than 2, then it is Virginica."

We simply provide many examples to the model.

The model learns these relationships automatically and uses them to make predictions on new, unseen data.

---

# 🎯 What is Classification?

Classification is a type of Machine Learning problem where the goal is to assign an item to one of several predefined categories.

Examples include:

- Detecting whether an email is Spam or Not Spam.
- Predicting whether a medical report is Positive or Negative.
- Identifying whether a handwritten digit is 0, 1, 2, or another number.
- Recognizing different types of flowers.

Our project is also a Classification problem because the model predicts one of three flower species.

---

# 🌼 What is the Iris Dataset?

The Iris Dataset is one of the most famous datasets in Machine Learning.

It was introduced by British statistician and biologist **Ronald A. Fisher** in 1936 and is commonly used to learn and practice classification algorithms.

The dataset contains information about **150 Iris flowers** belonging to **three different species**.

Each flower has four measurements:

| Feature | Description |
|----------|-------------|
| Sepal Length | Length of the sepal |
| Sepal Width | Width of the sepal |
| Petal Length | Length of the petal |
| Petal Width | Width of the petal |

The target variable is the flower species.

---

# 🌸 Iris Species

The dataset contains three different species of Iris flowers.

## 🌸 Iris Setosa

Setosa flowers have very small petals.

They are the easiest species to identify because their petal measurements are clearly different from the other two species.

---

## 🌺 Iris Versicolor

Versicolor flowers have medium-sized petals.

Their measurements fall between Setosa and Virginica.

---

## 🌼 Iris Virginica

Virginica flowers have the largest petals among all three species.

Because Versicolor and Virginica have similar characteristics, distinguishing between them is more challenging than identifying Setosa.

---

# 🌿 What are Sepals and Petals?

Every Iris flower has two important parts that were measured in this dataset.

## 🌿 Sepal

The sepal is the outer green part of a flower that protects the bud before it blooms.

In this dataset, two measurements are recorded:

- Sepal Length
- Sepal Width

---

## 🌺 Petal

The petal is the colorful part of a flower.

Petals play an important role in attracting pollinators such as bees and butterflies.

The dataset also records:

- Petal Length
- Petal Width

These four measurements become the **input features** for our Machine Learning model.

---

# 🧠 Why is this Project Important?

Although this project uses flowers as an example, the same Machine Learning concepts are used in many real-world applications.

The same classification techniques can be used for:

- Disease Detection
- Email Spam Detection
- Fraud Detection
- Face Recognition
- Sentiment Analysis
- Product Recommendation
- Customer Classification

That is why the Iris Dataset is considered one of the best beginner projects for understanding Machine Learning.

---

# 📊 Dataset Information

The Iris dataset contains **150 flower samples** collected from three different Iris species.

Each species has **50 samples**, making the dataset perfectly balanced for a classification problem.

The dataset consists of **5 columns**:

| Feature       | Description                   |
|---------------|-------------------------------|
| Sepal Length  | Length of the sepal (cm)      |
| Sepal Width   | Width of the sepal (cm)       |
| Petal Length  | Length of the petal (cm)      |
| Petal Width   | Width of the petal (cm)       |
| Species       | Target variable (Flower Type) |

### Dataset Summary

| Property           | Value     |
|--------------------|-----------|
| Total Samples      | 150       |
| Number of Features | 4         |
| Target Classes     | 3         |
| Missing Values     | None      |
| Data Type          | Numerical |

Since the dataset contains no missing values and is already clean, very little preprocessing was required before training the models.

---

# 🔍 Exploratory Data Analysis (EDA)

Before building any Machine Learning model, it is important to understand the data.

This process is called **Exploratory Data Analysis (EDA)**.

EDA helps us answer questions like:

- Which features are most useful?
- Are there any missing values?
- Are the classes balanced?
- Which variables have the strongest relationship?
- Can we visually separate the classes?

Understanding the data before training a model often leads to better decisions and better performance.

---

# 📈 Data Visualization

To understand the dataset better, different visualizations were created.

These plots helped reveal hidden patterns that cannot be seen by looking at numbers alone.

The visualizations included:

- Pair Plot
- Correlation Heatmap
- Histograms
- Box Plots

Each visualization provided valuable insights about the dataset.

---

# 🌸 Pair Plot Analysis

The Pair Plot compares every feature with every other feature.

It is one of the easiest ways to visualize how different classes are distributed.

### What I observed

✅ Petal Length clearly separated the three species.

✅ Petal Width also showed a very strong separation.

✅ Setosa formed its own distinct cluster.

✅ Versicolor and Virginica were closer to each other but still distinguishable.

### Why is this important?

The Pair Plot showed that **Petal Length** and **Petal Width** are the most informative features for classifying Iris flowers.

This observation became one of the key findings of this project.

---

# 🔥 Correlation Heatmap

A correlation heatmap was used to understand how different features are related to one another.

Correlation values range from **-1 to +1**.

- **+1** → Strong positive relationship
- **0** → No relationship
- **-1** → Strong negative relationship

The heatmap showed that:

- Petal Length and Petal Width have a strong positive correlation.
- Sepal Width contributes less compared to the petal features.
- Some features move together because they describe similar characteristics of the flower.

This analysis helped identify which features carry more useful information.

---

# 📦 Feature Selection

Machine Learning models learn from **features**.

In this project, the input features were:

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

The output (Target Variable) was:

- Species

The dataset was divided into:

```python
X = Features

y = Target
```

Where:

- **X** contains the flower measurements.
- **y** contains the correct flower species.

---

# ✂️ Train-Test Split

A Machine Learning model should not be tested on the same data it learns from.

To avoid this problem, the dataset was divided into two parts.

### Training Data

The model learns patterns from this data.

### Testing Data

The model is evaluated using data it has never seen before.

In this project, the dataset was divided into:

- **80% Training Data**
- **20% Testing Data**

This ensures that the evaluation is fair and realistic.

---

# 🤖 Model Training

After preparing the data, the Machine Learning models were trained.

Training is the stage where the model learns patterns from the dataset.

In Python, this happens using:

```python
model.fit(X_train, y_train)
```

This is one of the most important lines in the entire project.

When this line is executed, the model studies the relationship between the flower measurements and their correct species.

For example, it starts learning patterns such as:

- Flowers with very small petals are usually **Setosa**.
- Flowers with medium petals are often **Versicolor**.
- Flowers with larger petals are likely **Virginica**.

The model does **not memorize** the data.

Instead, it learns patterns that help it classify new flowers correctly.

---

# 🔮 Making Predictions

Once the model has completed training, it can predict the species of flowers it has never seen before.

Predictions are made using:

```python
model.predict(X_test)
```

Here, the model receives only the measurements of a flower.

It then analyzes those measurements and predicts whether the flower belongs to:

- 🌸 Setosa
- 🌺 Versicolor
- 🌼 Virginica

These predictions are then compared with the actual species to measure the model's performance.

---

# 🚀 Machine Learning Workflow

The complete workflow of this project is shown below:

```

Load Dataset

↓

Explore the Dataset (EDA)

↓

Visualize Patterns

↓

Select Features & Target

↓

Train-Test Split

↓

Train Machine Learning Models

↓

Make Predictions

↓

Evaluate Performance

↓

Compare Results

↓

Final Prediction

```

This workflow represents the complete Machine Learning pipeline followed in this project.

---

# 🤖 Machine Learning Models

To solve this classification problem, I trained and compared two supervised Machine Learning algorithms:

- Logistic Regression
- K-Nearest Neighbors (KNN)

Training multiple models helps compare their performance and choose the most suitable one for the given dataset.

---

# 🧠 Logistic Regression

Despite its name, Logistic Regression is mainly used for **classification problems**, not regression.

It predicts the probability that a sample belongs to a particular class.

In this project, Logistic Regression learned the relationship between the flower measurements and their corresponding species.

### Why Logistic Regression?

Some advantages of Logistic Regression include:

- Simple and easy to understand
- Fast training and prediction
- Works well on small and medium-sized datasets
- Easy to interpret
- Performs well when classes are clearly separated

For the Iris dataset, Logistic Regression performed exceptionally well because the flower species are naturally distinguishable using petal measurements.

---

# 👥 K-Nearest Neighbors (KNN)

K-Nearest Neighbors (KNN) is a distance-based Machine Learning algorithm.

Instead of learning mathematical equations, KNN compares a new sample with the most similar samples in the training dataset.

It then predicts the class based on the majority of its nearest neighbors.

### Real-Life Example

Imagine moving into a new neighborhood.

If most of your closest neighbors are doctors, you might assume the area has many medical professionals.

Similarly, KNN looks at the nearest data points and predicts the class based on the majority.

---

# ⚖️ Why Compare Multiple Models?

There is no single Machine Learning algorithm that performs best for every dataset.

Different datasets have different characteristics.

Comparing multiple models helps us understand:

- Which model performs better?
- Which model is easier to interpret?
- Which model is faster?
- Which model is more suitable for future use?

This is why both Logistic Regression and KNN were trained and evaluated.

---

# 📊 Model Performance

After training both models, their predictions were evaluated on the testing dataset.

| Model | Accuracy |
|--------|----------|
| Logistic Regression | 100% |
| K-Nearest Neighbors | 100% |

Both models classified every testing sample correctly.

However, accuracy alone does not always provide the complete picture.

Additional evaluation methods were also used.

---

# 📉 Confusion Matrix

A Confusion Matrix provides a detailed summary of the model's predictions.

Instead of showing only one number (accuracy), it tells us:

- How many flowers were classified correctly.
- Which species were confused with each other.
- Which predictions were correct or incorrect.

In this project, the Confusion Matrix showed that the models correctly classified all testing samples.

This result is consistent with the reported accuracy.

---

# 📋 Classification Report

The Classification Report provides more detailed evaluation metrics.

These include:

- Precision
- Recall
- F1-Score
- Support

### Precision

Precision measures how many predicted labels were actually correct.

### Recall

Recall measures how many actual samples were correctly identified.

### F1-Score

The F1-Score balances both Precision and Recall.

It is especially useful when comparing different classification models.

These metrics provide a deeper understanding of model performance beyond simple accuracy.

---

# 📈 Results

The final results showed that both Machine Learning models performed exceptionally well on the Iris dataset.

### Key Findings

✅ Both models achieved 100% testing accuracy.

✅ Petal Length and Petal Width were the most informative features.

✅ Setosa was the easiest species to classify because it formed a distinct cluster.

✅ Versicolor and Virginica shared similar characteristics, making them relatively closer than Setosa.

✅ The dataset contained no missing values, making preprocessing straightforward.

---

# 💡 Why Did Both Models Achieve 100% Accuracy?

One common question is:

> "How can two different algorithms produce the same accuracy?"

The answer lies in the dataset itself.

The Iris dataset is clean, balanced, and well-structured.

The flower species have clear differences, especially in petal measurements.

Because of these naturally separable patterns, multiple Machine Learning algorithms can achieve excellent performance.

This does **not** mean every real-world dataset will produce the same results.

Many practical datasets are noisy, imbalanced, and much more challenging.

---

# 🎯 Key Learnings

This project taught me much more than simply training a Machine Learning model.

Some of my biggest learnings were:

- Understanding the data is more important than immediately choosing an algorithm.
- Data visualization helps reveal patterns that numbers alone cannot show.
- Model evaluation should go beyond accuracy.
- Comparing multiple models provides better insights.
- A simple algorithm can perform extremely well when the data is clean and meaningful.

Overall, this project strengthened my understanding of the complete Machine Learning workflow—from data exploration to model evaluation.

---

# 📂 Project Structure

```
Iris-Flower-Classification/
│
├── Iris_Flower_Classification.ipynb
├── Iris.csv
├── README.md
├── requirements.txt
│
├── images/
│   ├── pairplot.png
│   ├── heatmap.png
│   ├── confusion_matrix.png
│   └── workflow.png
│
└── LICENSE
```

This structure keeps the project organized and makes it easier for others to understand and use.

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

---

### Step 4

Open the Jupyter Notebook.

```bash
jupyter notebook
```

Run all the cells and explore the project.

---

# 📸 Project Outputs

The project includes the following visualizations:

- Pair Plot
- Correlation Heatmap
- Confusion Matrix
- Classification Report
- Model Accuracy

> 📌 *You can add screenshots inside the `images` folder and display them here.*

Example:

```markdown
## Pair Plot

![Pair Plot](images/pairplot.png)

## Heatmap

![Heatmap](images/heatmap.png)

## Confusion Matrix

![Confusion Matrix](images/confusion_matrix.png)
```

---

# 🌍 Real-World Applications

Although this project classifies flowers, the same Machine Learning techniques are widely used in many real-world applications.

Examples include:

- 📧 Spam Email Detection
- 🏥 Disease Diagnosis
- 💳 Credit Card Fraud Detection
- 😊 Sentiment Analysis
- 👤 Face Recognition
- 📦 Product Recommendation Systems
- 🎵 Music Recommendation
- 🛒 Customer Segmentation

This project builds the foundation for understanding these more advanced applications.

---

# 🔮 Future Improvements

Some ideas to improve this project in the future:

- Train additional Machine Learning models.
- Perform Hyperparameter Tuning.
- Use Cross Validation.
- Deploy the model using Streamlit or Flask.
- Build a web application where users can enter flower measurements and receive predictions instantly.
- Experiment with larger and more complex datasets.

---

# 🎯 What I Learned

This project was my first hands-on experience with Machine Learning.

More importantly, it taught me that Machine Learning is not just about training models.

I learned how to:

- Understand a dataset before modeling.
- Explore data using EDA.
- Identify important features.
- Train different Machine Learning models.
- Compare multiple algorithms.
- Evaluate models using different metrics.
- Interpret the results instead of focusing only on accuracy.

This project strengthened my confidence in Data Science and encouraged me to continue learning more about Machine Learning.

---

# 🙏 Acknowledgements

This project was completed as part of the **Oasis Infobyte Data Science Internship**.

I would like to thank Oasis Infobyte for providing practical tasks that helped me apply Machine Learning concepts in a real project.

---

# 👩‍💻 Author

## **Palwasha**

**Data Science Student | Machine Learning Learner | Frontend Developer**

GitHub: [Palwasha-48](https://github.com/Palwasha-48)

LinkedIn: [Palwashey Qureshi](https://linkedin.com/in/palwasheyqureshi)
---

# ⭐ Support

If you found this project helpful, consider giving this repository a ⭐.

It motivates me to continue learning, building, and sharing more Data Science and Machine Learning projects.

Thank you for visiting my repository! 💙