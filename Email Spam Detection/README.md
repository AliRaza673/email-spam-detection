# 📩 Email Spam Detection with Logistic Regression

A machine learning project that detects whether an Email message is **spam** or **ham (not spam)**.  
The model uses **TF-IDF vectorization** with a **Logistic Regression** classifier and provides a simple **Gradio web interface** for real-time predictions.

---

## 🚀 Features
- Preprocesses text (lowercasing, URL removal, punctuation removal, stopword filtering).
- Converts messages into numerical features with **TF-IDF**.
- Trains a **Logistic Regression** model with class balancing.
- Evaluates performance with classification metrics and confusion matrix visualization.
- Saves both the trained model (`spam_model.pkl`) and TF-IDF vectorizer (`tfidf_vectorizer.pkl`).
- Provides a **Gradio web app** for easy message classification.

---

## 📂 Project Structure
email-spam-detection/
│── spam.csv # Dataset (not included here)
│── spam_model.pkl # Saved Logistic Regression model
│── tfidf_vectorizer.pkl # Saved TF-IDF vectorizer
│── app.py # Main training + Gradio app script
│── requirements.txt # Python dependencies
│── README.md # Project documentation



## 🛠 Installation

Clone this repository and install the required dependencies:

```bash
# Clone the repository
git clone https://github.com/your-username/email-spam-detection.git
cd email-spam-detection

# (Optional) Create virtual environment
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows

# Install dependencies
pip install -r requirements.txt
📊 Dataset
This project expects the dataset in CSV format. Example:

Columns: Category (spam/ham) and Message (text).

Commonly used dataset: UCI SMS Spam Collection Dataset

⚠️ Place your dataset in the project root or update the path inside app.py.

🏋️ Training the Model
Run the script to train and save the model:

bash
Copy code
python app.py
This will:

Preprocess the dataset

Train Logistic Regression

Evaluate performance with a classification report & confusion matrix

Save the trained model (spam_model.pkl) and vectorizer (tfidf_vectorizer.pkl)

🔍 Using the Gradio App
After training, launch the interactive spam detector:

bash
Copy code
python app.py
This will open a local Gradio interface in your browser:

Enter an Email message

Get prediction: Ham / Spam

See the spam probability score

Example:

vbnet
Copy code
Input: "Congratulations! You have won a free ticket."
Output: Spam, 0.97
📈 Results
Algorithm: Logistic Regression

Evaluation:

Precision, Recall, F1 reported via classification_report

Confusion matrix visualization included

Typical Accuracy: ~95% (varies by dataset)

📜 License
This project is licensed under the MIT License – feel free to use, modify, and distribute.

🤝 Contributing
Pull requests and feature suggestions are welcome.
If you’d like to add new models (e.g., Naive Bayes, SVM, or Deep Learning), feel free to contribute!


---

👉 Save this as `README.md` in your **project root folder**.  
When you push it to GitHub, it will automatically show up as the homepage of your repo.  

