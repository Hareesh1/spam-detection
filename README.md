#📧 Spam Mail Detection Using Logistic Regression

This project implements a machine learning model to classify SMS messages as either spam or ham (non-spam) using logistic regression and TF-IDF vectorization.

📂 Dataset

The dataset used is spam.csv, which contains labeled SMS messages:

v1: Label (spam or ham)

v2: Message content

Additional unnamed columns are dropped during preprocessing.

🧪 Libraries Used

pandas for data manipulation

matplotlib and seaborn for visualization

sklearn for model building and evaluation

TfidfVectorizer for text feature extraction

🔍 Workflow

Load and Inspect Data

Read CSV with proper encoding

Display basic info and head of the dataset

Data Cleaning

Replace nulls with empty strings

Drop unnecessary columns (Unnamed: 3, Unnamed: 4)

Encode labels: spam → 0, ham → 1

Visualization

Count plot of spam vs ham messages

Feature Extraction

Use TfidfVectorizer to convert text into numerical features

Model Training

Split data into training and test sets (80/20)

Train a LogisticRegression model

Evaluation

Measure accuracy on both training and test sets

Prediction

Input a new message and predict whether it's spam or ham

📈 Accuracy

Training Accuracy: ~ (depends on run)

Test Accuracy: ~ (depends on run)

🧪 Example Prediction

input_mail = ['WINNER!! As a valued network customer you have been selected to receive a £900 prize reward!']

Output:

spam mail

🚀 How to Run

Clone the repository or copy the script.

Ensure spam.csv is placed in the correct path.

Install required libraries:

pip install pandas scikit-learn matplotlib seaborn

Run the script in a Python environment.

📌 Notes

Encoding is set to ISO-8859-1 to handle special characters.

TF-IDF helps reduce the impact of common stop words.

Logistic Regression is chosen for its simplicity and interpretability.
