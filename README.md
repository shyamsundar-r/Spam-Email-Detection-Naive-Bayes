## Spam Detection using Naive Bayes
This project is a simple spam message classifier built using Python's Scikit-learn library. It uses a Multinomial Naive Bayes model combined with a Count Vectorizer to classify text messages as either Spam or Ham (Not Spam).

## Table of Contents
- [Overview](#Overview)
- [Technologies Used](#Technologies-Used)
- [Dataset](#Dataset)
- [Installation](#Installation)
- [Usage](#Usage)
- [Example Output](#Example-Output)
- [Model Explanation](#Model-Explanation)
- [Results](#Results)
- [License](#License)
  
## Overview
- Load and preprocess a dataset (spam.csv)
- Encode labels (Spam and Ham) into numerical format
- Split data into training and test sets
- Train a Naive Bayes classifier
- Evaluate the model using accuracy, confusion matrix, and classification report
- Predict user-input messages in real-time via the command line

## Technologies Used
- Python
- Pandas
- Scikit-learn
- Seaborn
- Matplotlib

## Dataset
- The dataset used is he Email Spam Collection Dataset available on Kaggle:
[Download from Kaggle spam.csv](https://www.kaggle.com/datasets/mfaisalqureshi/spam-email)
- spam.csv, which should contain at least two columns:
  - Category: Label of the message (Spam or Ham)
  -  Message: The actual text content of the message

## Installation
1. Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/Spam-Detection-NaiveBayes.git
cd Spam-Detection-NaiveBayes
2. Install required libraries:

bash
Copy
Edit
pip install pandas numpy scikit-learn matplotlib seaborn

## Usage
1. Run the script
2. After training, enter a message to check if it’s spam or not.
3. Type exit to quit.


## Example Output
pgsql
Copy
Edit
Enter a message to check (or type 'exit' to quit): Win a free iPhone now!
'Win a free iPhone now!' => Spam

Enter a message to check (or type 'exit' to quit): Hello, how are you?
'Hello, how are you?' => Ham

## Model Explanation
- Algorithm Used: Multinomial Naive Bayes
- Vectorization: CountVectorizer (converts text to token count matrix)
- Label Encoding: Spam = 1, Ham = 0
- Pipeline: Combines preprocessing and modeling for efficient prediction

## Results
- Accuracy: ~97–99% (depending on data split)
- Evaluation Metrics:
  - Accuracy Score
  - Confusion Matrix (with heatmap)
  - Classification Report (Precision, Recall, F1-score)

## License
This project is open-source and available under the MIT License.
