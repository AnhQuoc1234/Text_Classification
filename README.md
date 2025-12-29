Overview
This Jupyter Notebook implements a text classification model using Naive Bayes to categorize text data into predefined labels (e.g., Technology, Sports, Politics, Entertainment). It uses a synthetic dataset to train and evaluate the model's performance.

Features
Data Loading: Reads text data from a CSV file (synthetic_text_data.csv).

Preprocessing: Converts raw text into numerical vectors using CountVectorizer.

Model Training: Trains a MultinomialNB (Multinomial Naive Bayes) classifier.

Evaluation: Calculates accuracy and displays a confusion matrix heatmap.

Inference: Includes a script to classify custom user input strings.

Dependencies
To run this notebook, you need the following Python libraries installed:

Bash

pip install pandas numpy scikit-learn matplotlib seaborn tensorflow streamlit
Note: tensorflow and streamlit are imported in the notebook, potentially for future extensions or deployment.

Dataset
The notebook expects a dataset named synthetic_text_data.csv containing at least two columns:

text: The content to be classified.

label: The category of the text.

Important: You may need to update the file path in the code df = pd.read_csv(...) to match the location of your dataset.

Usage
Load the Data: Run the initial cells to load and inspect the dataframe.

Train the Model: The notebook splits the data (80% train, 20% test) and fits the Naive Bayes model.

Evaluate:

The model achieves an accuracy of approximately 88% on the test set.

A confusion matrix heatmap is generated to visualize performance across classes.

Make Predictions:

Scroll to the bottom of the notebook to test custom sentences.

Example: Inputting "I love artificial intelligence and machine learning" predicts the label 'Technology'.
