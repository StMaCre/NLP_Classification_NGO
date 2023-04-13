# NLP_Classification_NGO

# NGO Activity Classification
This project aims to classify non-governmental organizations (NGOs) into one of nine categories based on their name and description. The dataset contains information on approximately 8000 NGOs.

## Project Structure
The project is divided into two parts:


Import necessary libraries and read the data from the provided dataset.

Clean the dataset by removing unnecessary columns and dropping rows with missing values.

Label the data by creating a dictionary of categories and their corresponding keywords.

Create new columns in the DataFrame to store the count of keywords in each category.

Iterate over the rows of the DataFrame, calculate the count of keywords in each category, and store the results in the corresponding columns.

Load the Spanish language model from SpaCy.

Clean the labels and remove stop words from the text using NLTK.

Add a custom text categorizer to the SpaCy pipeline.

Preprocess the data by removing stop words and create new columns in the Mexico DataFrame to store the predicted activity probabilities.

Iterate over the rows of the DataFrame, process the text, and store the probabilities in the corresponding columns.

Create a dictionary of label titles and add new columns to the DataFrame to store the predicted title probabilities.

Iterate over the rows of the DataFrame again, process the titles, and store the probabilities in the corresponding columns.

Create new columns in the DataFrame to store the sum of activities corresponding to each category.

Prepare the data for training a classifier by removing unnecessary columns and one-hot encoding the target variable.

Split the data into training and testing sets.

Train a RandomForestClassifier and evaluate its performance on the test set.

Train an XGBoost classifier and evaluate its performance on the test set.

# Results
The RandomForestClassifier obtains an accuracy score of 0.81 and the XGBoost classifier achieves an accuracy score of 0.9302 on the test set.
