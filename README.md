# EMAIL_SPAM_DETECTOR
This is a simple email spam detector program that classifies emails as either spam or not spam (ham). The program uses a machine learning model trained on a dataset of labeled emails to make predictions.

Email Spam Detector
Overview
This is a simple email spam detector program that classifies emails as either spam or not spam (ham). The program uses a machine learning model trained on a dataset of labeled emails to make predictions.

Requirements
Python 3.x
Libraries:
scikit-learn
pandas
numpy
nltk

Installation
Clone or download the repository to your local machine.
Install the required libraries using pip:
Copy code
pip install -r requirements.txt
Download NLTK data by running the following Python script:
python
Copy code
import nltk
nltk.download('stopwords')
nltk.download('punkt')

Usage
Prepare your email dataset in CSV format with two columns: text (email content) and label (0 for ham, 1 for spam).
Put your dataset in the data directory.
Train the model by running:
css
Copy code
python train.py --input <path_to_your_dataset.csv> --output <path_to_save_model.pkl>
Once the model is trained, you can use it to classify emails:
css
Copy code
python classify.py --model <path_to_saved_model.pkl> --email "Your email content goes here"
Replace "Your email content goes here" with the actual email content you want to classify.

Acknowledgments
The dataset used for training the model is from the UCI Machine Learning Repository.
This project is inspired by various online tutorials and resources.

License
This project is licensed under the MIT License - see the LICENSE file for details.
