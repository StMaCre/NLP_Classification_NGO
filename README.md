# NLP_Classification_NGO

# NGO Activity Classification
This project aims to classify non-governmental organizations (NGOs) into one of nine categories based on their name and description. The dataset contains information on approximately 8000 NGOs.

## Project Structure
The project is divided into different parts:

### I. Data Preparation
A. Import Libraries and Load Dataset

B. Clean Dataset
- 1. Remove Unnecessary Columns
- 2. Drop Rows with Missing Values

### II. Data Labeling
A. Create Category Dictionary with Keywords
B. Add Columns for Keyword Counts
- 1. Calculate Keyword Counts per Category
- 2. Store Keyword Counts in Columns

### III. Text Preprocessing
A. Clean Labels and Remove Stop Words with NLTK
B. Add Custom Text Categorizer to SpaCy Pipeline
C. Preprocess Data
- 1. Remove Stop Words
- 2. Add Columns for Predicted Activity Probabilities
- 3. Store Probabilities in Columns

### IV. Title Processing
A. Create Label Titles Dictionary
B. Add Columns for Predicted Title Probabilities
- 1. Process Titles
- 2. Store Probabilities in Columns

### V. Sum of Activities
A. Add Columns for Sum of Activities per Category

### VI. Classifier Training Preparation
A. Remove Unnecessary Columns
B. One-hot Encode Target Variable

### VII. Model Training and Evaluation
A. RandomForestClassifier
- 1. Train Model
- 2. Evaluate Performance on Test Set
B. XGBoost Classifier
- 1. Train Model
- 2. Evaluate Performance on Test Set

# Results
The RandomForestClassifier obtains an accuracy score of 0.81 and the XGBoost classifier achieves an accuracy score of 0.9302 on the test set.
