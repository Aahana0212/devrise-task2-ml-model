# Iris Classification - Machine Learning Model

DevRise Internship Program - Batch 1 (2026) | Domain: AI & ML | Task 2

## Project Overview
This project builds an end-to-end machine learning classification pipeline
on the classic Iris dataset, comparing Logistic Regression, Decision Tree,
and Random Forest classifiers, and evaluating their performance using
standard classification metrics.

## Objective
- Clean and profile the Iris dataset features
- Split data into training and test sets (stratified, leakage-free)
- Train multiple classifiers using Scikit-Learn
- Evaluate models using Accuracy, Precision, Recall, F1-Score, and Confusion Matrix
- Visualize feature distributions, pairwise relationships, and decision boundaries

## Project Structure
DevRise-Task2/
- Task2_ML_Model.ipynb (Main Jupyter Notebook)
- plots/ (Exported high-resolution plots)
- README.md (This file)

## Setup Instructions
1. Clone the repository
   git clone <your-repo-url>
   cd DevRise-Task2

2. Install dependencies
   pip install scikit-learn pandas numpy matplotlib seaborn jupyter

3. Launch Jupyter Notebook
   jupyter notebook Task2_ML_Model.ipynb

4. Run all cells (Kernel > Restart & Run All) to reproduce the analysis.

## Dataset
The classic Iris dataset (150 samples, 4 features, 3 balanced classes) is
loaded directly via sklearn.datasets.load_iris(). Features: sepal length,
sepal width, petal length, petal width. Target: species
(setosa / versicolor / virginica).

## Pipeline Summary
- Data profiling: checked for missing values, duplicates, class balance
- Feature exploration: histograms, pair plot, correlation heatmap
- Train/Test split: 80/20 stratified split, random_state=42
- Feature scaling: StandardScaler fit on training data only (no leakage)
- Models trained: Logistic Regression, Decision Tree, Random Forest
- Evaluation: Accuracy, Precision, Recall, F1-Score, Confusion Matrix
- Visualization: Confusion matrix heatmaps, model comparison chart, decision boundary plot

## Key Insights
- All three models achieved 93.3% accuracy, since Iris classes are well separated in feature space.
- Petal length and petal width are the most discriminative features.
- Setosa is almost always perfectly classified; most misclassifications occur between versicolor and virginica.
- One duplicate row was found and removed during data cleaning; no missing values were present.

## Demo Video
[Demo Video Link](your-video-link-here)

## Tech Stack
- Python 3
- Scikit-Learn
- Pandas / NumPy
- Matplotlib / Seaborn
- Jupyter Notebook

## Author Name
Ahana Singh - DevRise Internship, Batch 1 (2026)