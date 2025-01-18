# Car-Price-Prediction

# Car Price Predictor

This is a **Flask-based web application** that predicts the price of a car based on its features, such as the manufacturer, model, year, fuel type, and kilometers driven. The application uses a pre-trained **Linear Regression model** for predictions.

---

## Features

- Predict car prices using machine learning.
- Dynamic dropdowns for selecting manufacturers, models, and other details.
- User-friendly interface built with **Bootstrap 4**.
- Asynchronous form submission using **AJAX** for real-time predictions.

---

## Tech Stack

### Backend:
- **Python 3**
- **Flask** for routing and serving the web application.
- **Pickle** for loading the pre-trained model.
- **pandas** for data handling.

### Frontend:
- **HTML5** and **CSS** for structuring and styling.
- **Bootstrap 4** for responsive design.
- **JavaScript** for dynamic behaviors and AJAX.

### Machine Learning:
- **Linear Regression** (trained using **scikit-learn**) to predict car prices based on input features.

---

## Dataset

The model is trained on a cleaned dataset of car sales (`Cleaned_Car_data.csv`). It contains the following features:
- Manufacturer (`company`)
- Model (`name`)
- Year of manufacture (`year`)
- Fuel type (`fuel_type`)
- Kilometers driven (`kms_driven`)
- Selling price (`price`) as the target variable.

---

## Installation

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/car-price-predictor.git
cd car-price-predictor
```

### 2. Install Dependencies
Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # For Linux/Mac
venv\Scripts\activate     # For Windows
```

Install required Python libraries:
```bash
pip install -r requirements.txt
```

### 3. Run the Application
Start the Flask development server:
```bash
python app.py
```

Open the app in your browser:
```
http://127.0.0.1:5000/
```

---

## File Structure

```plaintext
car-price-predictor/
│
├── static/
│   ├── css/
│   │   └── stylesheet.css
│   └── ...
│
├── templates/
│   ├── index.html
│
├── app.py                # Main Flask application
├── LinearRegressionModel.pkl  # Pre-trained model file
├── Cleaned_Car_data.csv  # Dataset for the application
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```

---

## How It Works

1. Users select the manufacturer, model, year, fuel type, and input kilometers driven.
2. The data is sent to the Flask server via AJAX.
3. The server processes the data, uses the trained model to predict the price, and sends the prediction back to the client.
4. The predicted price is displayed in real-time without reloading the page.

   
## Future Enhancements

- Add support for additional machine learning models (e.g., Random Forest, Gradient Boosting).
- Include features like car color, transmission type, and engine size for more accurate predictions.
- Extend the application to support multiple languages.
- Deploy the application using platforms like **Heroku** or **AWS**.

