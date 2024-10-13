# CancerPredictorApplication

## Overview
CancerPredictorApplication is a machine learning-based web application designed to predict the likelihood of breast cancer based on medical data. Using a trained decision tree classifier, the application takes input from the user and provides a prediction indicating whether or not the individual is at risk of breast cancer.

## Features
- Predicts breast cancer likelihood using a decision tree classifier.
- User-friendly web interface for inputting medical data.
- Instant feedback on cancer risk after data submission.

## Technologies Used
- **Python**: Core programming language.
- **Flask**: Web framework used to build the web interface.
- **Pandas**: For data manipulation and reading CSV files.
- **Scikit-learn**: For machine learning (Decision Tree Classifier).
- **HTML**: To create the web interface.

## Dataset
The application uses a dataset (`dataR2.csv`) containing medical features such as:
- Age
- BMI (Body Mass Index)
- Glucose
- Insulin
- HOMA
- Leptin
- Adiponectin
- Resistin
- MCP.1
- Classification (target variable)

The model is trained on this data to predict the classification, which indicates the presence or absence of breast cancer.

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/CancerPredictorApplication.git
   cd CancerPredictorApplication
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Place the dataset (`dataR2.csv`) in the root folder.
4. Run the Flask application:
   ```bash
   python app.py
   ```
5. Open your browser and navigate to `http://127.0.0.1:5000/`.
6. Fill in the form with the required medical data and submit to see the prediction.

## Output
![Screenshot (310)](https://github.com/user-attachments/assets/2e3f349b-49a1-4bbe-ac6e-1ccf4159a685)

## Project Structure
```
CancerPredictorApplication/
│
├── templates/
│   └── index.html        # HTML file for the web interface
├── app.py                # Main Flask application file
├── dataR2.csv            # Medical dataset used for training
├── requirements.txt      # Python dependencies
└── README.md             # This README file
```

## Future Enhancements
- Improve the model by testing other algorithms (e.g., SVM, Naive Bayes).
- Add data validation and error handling for form inputs.
- Use a database to store user inputs and prediction results.

## License
This project is open-source and available under the MIT License.

