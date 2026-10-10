# Diabetes Prediction Using Decision Tree Classifier

## 📌 Project Overview
This project uses a **Decision Tree Classification** algorithm to predict whether a person has diabetes based on the input features available in the diabetes dataset.

The project is implemented in Python using Jupyter Notebook and the Scikit-learn machine learning library. It includes data loading, preprocessing, model training, performance evaluation, hyperparameter tuning, and saving the trained model.

## 🎯 Project Objectives
- Understand the Decision Tree Classification algorithm.
- Load and explore the diabetes dataset using Pandas.
- Split the dataset into training and testing sets.
- Train a Decision Tree Classifier.
- Evaluate the model using accuracy, a confusion matrix, and a classification report.
- Improve model performance using GridSearchCV.
- Save the trained model for future use.

## 🛠️ Technologies Used
- **Python** – Programming language
- **Jupyter Notebook** – Development environment
- **NumPy** – Numerical operations
- **Pandas** – Data manipulation and analysis
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Scikit-learn** – Machine learning and model evaluation
- **Pickle** – Saving the trained model and feature names

## 📂 Dataset
The project uses a CSV file named `diabetes.csv`.

The target column is:
- `Outcome` – Represents the classification target.

The input features are all columns except `Outcome`.

The dataset must be placed in the appropriate working directory before running the notebook.

## ⚙️ Project Workflow

1. Import the required Python libraries.
2. Load the dataset using Pandas.
3. Explore the dataset using `head()` and `info()`.
4. Separate the input features (`X`) and target variable (`y`).
5. Visualize the distribution of the target variable.
6. Split the data into training and testing sets using an 80:20 ratio.
7. Train a Decision Tree Classifier using the Gini criterion.
8. Evaluate training and testing performance.
9. Tune model hyperparameters using GridSearchCV with 5-fold cross-validation.
10. Train an optimized Decision Tree model.
11. Evaluate the optimized model.
12. Save the trained model and feature names as pickle files.

## 🤖 Machine Learning Algorithm

### Decision Tree Classifier
A Decision Tree is a supervised machine learning algorithm that makes predictions by learning decision rules from the input features.

The initial model uses:

`DecisionTreeClassifier(criterion='gini')`

### Hyperparameter Tuning
GridSearchCV is used to explore different combinations of:
- `criterion`: Gini and entropy
- `max_depth`: Tree depth
- `min_samples_split`: Minimum samples required to split a node
- `min_samples_leaf`: Minimum samples required at a leaf node

The notebook uses 5-fold cross-validation to compare parameter combinations.

## 📊 Model Evaluation
The project evaluates the classifier using the following metrics:

- **Accuracy Score:** Measures the proportion of correct predictions.
- **Confusion Matrix:** Shows correct and incorrect classifications.
- **Classification Report:** Provides precision, recall, F1-score, and support.

Both the initial and tuned models are evaluated on training and testing data.

*Note: Actual accuracy and other performance values should be taken from the notebook output.*

## 💾 Saved Model Files
After executing the model-saving cell, the project creates:

- `diabetes_model.pkl` – Stores the trained Decision Tree model.
- `diabetes_features.pkl` – Stores the names of the input features.

These files can be used in a future prediction application, provided the input data matches the model's expected features.

## 🚀 How to Run the Project

### 1. Clone the repository
```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd YOUR_PROJECT_FOLDER
```

Replace the placeholders with your actual GitHub repository URL and folder name.

### 2. Install the required libraries
```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

### 3. Add the dataset
Place `diabetes.csv` in the notebook's working directory.

### 4. Open Jupyter Notebook
```bash
jupyter notebook
```

### 5. Run the notebook
Open `Day 58_Decision Tree Diabetes Data.ipynb` and execute the cells in order.

## 📁 Project Structure
```text
Diabetes-Prediction/
│
├── Day 58_Decision Tree Diabetes Data.ipynb
├── diabetes.csv
├── diabetes_model.pkl
├── diabetes_features.pkl
└── README.md
```

The two pickle files are generated when the model-saving cell is executed.

## 🔮 Future Improvements
- Evaluate additional classification algorithms.
- Compare model performance using appropriate evaluation metrics.
- Visualize the trained Decision Tree.
- Build a simple web application for predictions.
- Validate the model on suitable independent data.

## ⚠️ Disclaimer
This project is for educational and machine learning practice purposes only. Its predictions should not be used as a substitute for professional medical advice or diagnosis.

## 👨‍💻 Author
**Sanket Bacche**

Artificial Intelligence and Data Science Student

## ⭐ Conclusion
This project demonstrates how a Decision Tree Classifier can be trained and evaluated on a diabetes dataset. It also introduces hyperparameter tuning with GridSearchCV and saving a trained model for future use.
