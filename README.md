📧 Spam Email Classifier
This project is a machine learning-based spam email classifier using logistic regression. It leverages key email features to determine whether an email is spam or not.

🧰 Libraries & Algorithm Used
🧪 Python Libraries
pandas – Data manipulation and loading CSV files

seaborn – Data visualization (e.g., pair plots and heatmaps)

matplotlib – Plot rendering

scikit-learn – Machine learning tools:

LabelEncoder – Converts string labels ("yes"/"no") to numeric format (0/1)

StandardScaler – Feature normalization

train_test_split – Splitting dataset into training and test sets

LogisticRegression – ML model for classification

classification_report & confusion_matrix – Evaluation metrics

cross_val_score – Cross-validation performance

🤖 Machine Learning Algorithm
Logistic Regression
A simple and efficient algorithm used for binary classification tasks. It estimates the probability that a given input belongs to a particular category (in this case: spam or not spam).

📁 Dataset
The dataset used is spam_emails.csv, which should contain the following columns:

num_links (int)

num_attachments (int)

sender_reputation (float)

is_spam (categorical: "yes"/"no")

🧠 Workflow Summary
Data Loading & Preprocessing

Load dataset with Pandas

Encode is_spam label using LabelEncoder

Standardize features with StandardScaler

Visualization

Use seaborn.pairplot to visualize feature distributions grouped by spam labels

Model Training

Split dataset into train and test sets

Train a logistic regression model on the scaled features

Evaluation

Evaluate model performance with a classification report and confusion matrix

Perform 5-fold cross-validation to assess average accuracy

📊 Results
The model prints:

Classification Report: Precision, recall, f1-score, and support for each class

Confusion Matrix: Visual representation of prediction vs. actual

Cross-validation Accuracy: Mean accuracy across 5 folds

📈 Sample Output
text
Copy
Edit
Classification Report on Test Set:
              precision    recall  f1-score   support

          no       0.88      0.90      0.89        60
         yes       0.87      0.85      0.86        50

    accuracy                           0.88       110
   macro avg       0.88      0.87      0.87       110
weighted avg       0.88      0.88      0.88       110

Average Cross-Validation Accuracy: 0.87
