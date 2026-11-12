# Breast Cancer Classification Using Machine Learning

## Project Description

This project applies machine-learning techniques to classify breast tumours as benign or malignant using the UCI Breast Cancer Wisconsin Diagnostic dataset.

The project compares traditional machine-learning models with a neural network and evaluates their ability to identify malignant tumours accurately.

## Project Objectives

The objectives of this project are to:

1. Clean and explore the breast cancer dataset.
2. Prepare the data for machine-learning analysis.
3. Develop and train several classification models.
4. Optimize model hyperparameters using cross-validation.
5. Compare traditional machine-learning models with a neural network.
6. Identify the model with the most suitable performance.

## Dataset

The project uses the UCI Breast Cancer Wisconsin Diagnostic dataset.

The dataset contains:

- 569 observations.
- One identification variable.
- One diagnosis variable.
- 30 numerical tumour-measurement features.

The diagnosis variable is coded as follows:

- `B`: Benign tumour.
- `M`: Malignant tumour.

The identification column is removed during data preparation because it does not provide meaningful predictive information.

## Machine-Learning Models

The following models are developed and compared:

- Logistic Regression.
- Support Vector Machine.
- Random Forest.
- Neural Network.

The neural network is included because it is a mandatory requirement of the project.

## Data Preparation

The project workflow includes:

- Checking the dataset structure.
- Checking for missing values.
- Checking for duplicate observations.
- Encoding the diagnosis variable.
- Removing the identification column.
- Scaling numerical variables where required.
- Exploring feature relationships and target distribution.
- Identifying important predictive features.

## Data Splitting

The dataset is divided into three stratified subsets:

- 70% training data.
- 15% validation data.
- 15% test data.

The training set is used to develop the models, the validation set is used to compare model performance during development, and the test set is used only for final evaluation.

## Hyperparameter Optimization

Hyperparameters are optimized using five-fold stratified cross-validation. Grid search is used to test suitable combinations of model parameters while keeping the test set separate from the development process.

The neural network uses early stopping to reduce the risk of overfitting. Training and validation loss and accuracy curves are included in the notebook.

## Evaluation Metrics

The models are evaluated using:

- Accuracy.
- Precision.
- Recall.
- F1-score.
- ROC-AUC.
- Confusion matrix.

Recall is particularly important because failing to identify a malignant tumour as malignant may have serious consequences.

## Repository Files

```text
breast-cancer-classification-ml-project/
│
├── Breast_Cancer_Classification_ML_Project.ipynb
├── wdbc.data
├── wdbc.names
├── README.md
├── requirements.txt
│
└── figures/
    ├── target_distribution.png
    ├── correlation_heatmap.png
    ├── neural_network_curves.png
    └── roc_curves.png
```

## File Descriptions

- `Breast_Cancer_Classification_ML_Project.ipynb`: Complete project notebook containing the code, analysis, visualizations and results.
- `wdbc.data`: Breast cancer dataset used for the analysis.
- `wdbc.names`: Official description of the dataset and its variables.
- `requirements.txt`: Python libraries required to run the notebook.
- `figures/`: Visualizations generated during the analysis.

## How to Run the Project

1. Download or clone this repository.
2. Install the required Python libraries listed in `requirements.txt`.
3. Open `Breast_Cancer_Classification_ML_Project.ipynb` in Jupyter Notebook or Google Colab.
4. Ensure that `wdbc.data` is in the same directory as the notebook.
5. Run the notebook cells from beginning to end.

## Expected Outputs

The notebook produces:

- Dataset summaries.
- Exploratory data-analysis graphs.
- Feature-correlation analysis.
- Hyperparameter results.
- Neural-network training and validation curves.
- Confusion matrices.
- ROC curves.
- A final model-comparison table.

## Project Repository

```text
https://github.com/daehcae-hub/breast-cancer-classification-ml-project
```

