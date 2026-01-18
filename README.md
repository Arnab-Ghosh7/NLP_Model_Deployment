# NLP Model Deployment - SMS Spam Validator

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Flask](https://img.shields.io/badge/Flask-Web%20Framework-lightgrey)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange)






## 🚀 Features

- **Real-time Prediction**: Instantly classify SMS messages as Spam or Ham.
- **Web Interface**: User-friendly web UI built with Flask and HTML/CSS.
- **Machine Learning**: Utilizes a Naive Bayes classifier (MultinomialNB) trained on a labeled dataset.
- **Text Preprocessing**: Implements CountVectorizer for feature extraction from text data.

## 🛠️ Tech Stack

- **Python**: Core programming language.
- **Flask**: Web framework for serving the application.
- **Pandas**: Data manipulation and analysis.
- **Scikit-learn**: Machine learning library for model training and vectorization.

## 📂 Project Structure

```
NLP_Model_Deployment/
├── app.py              # Main Flask application
├── spam.csv            # Dataset used for training
├── static/             # CSS and static assets
├── templates/          # HTML templates (home.html, result.html)
└── README.md           # Project documentation
```

## 🔧 Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Arnab-Ghosh7/NLP_Model_Deployment
    cd NLP_Model_Deployment
    ```

2.  **Install dependencies:**
    It is recommended to use a virtual environment.
    ```bash
    pip install flask pandas scikit-learn
    ```
    *(Note: If you have a `requirements.txt` file, you can run `pip install -r requirements.txt` instead.)*

## 💡 Usage

1.  **Run the application:**
    ```bash
    python app.py
    ```

2.  **Access the web interface:**
    Open your web browser and go to:
    `http://127.0.0.1:5000/`

3.  **Test the model:**
    - Enter a sample SMS message in the text box.
    - Click the "Predict" button.
    - View the result (Spam or Ham).

## 📊 Model Details

The application trains a **Multinomial Naive Bayes** classifier on startup using the provided `spam.csv` dataset.
- **Dataset**: A collection of SMS messages labeled as `spam` or `ham`.
- **Preprocessing**: Messages are tokenized and converted into a bag-of-words model using `CountVectorizer`.
- **Training**: The model is trained on 67% of the data, with 33% reserved for testing (internal validation).



## 📄 License

This project is licensed under the [MIT License](LICENSE).


## Author
Arnab Ghosh
