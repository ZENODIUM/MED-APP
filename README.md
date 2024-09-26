# Care Companion AI
# Medical Application: Disease Prediction and Medical Chatbot
https://www.kaggle.com/code/vizeno/pneumonia-image-classification-cnn-gradcam - Pneumonia Model File
## Overview
This repository contains a comprehensive medical application designed to predict various diseases and provide interactive medical assistance using a chatbot powered by GPT-2. The application features:

- **Disease Prediction**: Upload patient data and get predictions for common diseases using machine learning models.
- **Medical Chatbot**: Interact with a medical chatbot for basic inquiries, health tips, and explanations powered by GPT-2.
- **User-Friendly Interface**: Built using Streamlit for a clean, easy-to-navigate interface.

## Features
1. **Disease Prediction Module**:
    - Supports multiple diseases like diabetes, heart disease, and breast cancer.
    - Model architectures include Random Forest, SVM, and Neural Networks.
    - Allows users to upload CSV files for batch predictions.
    - Displays prediction results with probability scores.

2. **Medical Chatbot**:
    - Based on GPT-2, this chatbot can answer general health questions.
    - Can provide recommendations and engage in basic health-related conversations.
  
3. **Interactive Dashboard**:
    - Provides visual insights and graphs for the uploaded patient data.
    - Shows prediction distribution and data correlation.

4. **Model Performance**:
    - Displays evaluation metrics such as accuracy, precision, recall, and F1-score.
    - Allows comparison between different machine learning models.
  
## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/medical-application.git
    cd medical-application
    ```

2. Create a virtual environment:
    ```bash
    python -m venv env
    source env/bin/activate  # For Windows use `env\Scripts\activate`
    ```

3. Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Run the application:
    ```bash
    streamlit run app.py
    ```

## Dependencies
Make sure to have the following libraries installed:

- `streamlit`
- `pandas`
- `numpy`
- `scikit-learn`
- `tensorflow`
- `torch`
- `transformers`
- `matplotlib`
- `seaborn`
- `joblib`
- `requests`

These can be installed through the `requirements.txt` file provided in the repository.

## Project Structure
The project is organized as follows:

```plaintext
medical-application/
├── app.py                  # Main Streamlit application
├── chatbot/
│   ├── chatbot.py          # Chatbot implementation using GPT-2
│   └── gpt2_model/         # GPT-2 model files
├── disease_prediction/
│   ├── heart_disease.py    # Heart disease prediction logic
│   ├── diabetes.py         # Diabetes prediction logic
│   └── breast_cancer.py    # Breast cancer prediction logic
├── data/
│   └── sample_data.csv     # Sample data for testing
├── models/
│   ├── heart_disease.pkl   # Pretrained model for heart disease
│   ├── diabetes.pkl        # Pretrained model for diabetes
│   └── breast_cancer.pkl   # Pretrained model for breast cancer
├── requirements.txt        # Required packages for the project
└── README.md               # Project documentation
```

## Usage Guide

### 1. Disease Prediction
- **Upload Data**: Navigate to the `Disease Prediction` section and upload your CSV file.
- **Select Disease**: Choose the disease model (e.g., Heart Disease, Diabetes).
- **Get Predictions**: Click `Predict` to view the results.

### 2. Chatbot Assistance
- Navigate to the `Medical Chatbot` section.
- Type your query in the text box.
- Press `Enter` to receive a response from the GPT-2 chatbot.

### Model Training
To retrain the models, follow these steps:

1. **Prepare the Dataset**: Place your dataset in the `data/` folder.
2. **Modify the Script**: Update the corresponding script in the `disease_prediction/` folder.
3. **Train and Save the Model**:

    ```bash
    python disease_prediction/heart_disease.py
    ```

    The newly trained model will be saved in the `models/` directory.

## Contribution
Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch:

    ```bash
    git checkout -b feature/your-feature-name
    ```

3. Make your changes and commit them:

    ```bash
    git commit -m "Add new feature"
    ```

4. Push to the branch:

    ```bash
    git push origin feature/your-feature-name
    ```

5. Open a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.



