# Mental Health Prediction Using Smartphone Usage

This project is a Django web application that predicts mental health status based on smartphone usage data. It uses a machine learning model trained on usage patterns such as screen time, call logs, and message frequency.

## Features

- User input form for smartphone usage data
- Predicts mental health status using a pre-trained model (`mental_health_model.pkl`)
- Stores usage data in a SQLite database
- Simple web interface

## Project Structure

```
mental_health_predictor/
├── dataset.csv
├── db.sqlite3
├── manage.py
├── mental_health_model.pkl
├── README.md
├── mental_health_predictor/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
├── predictions/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── tests.py
│   ├── views.py
│   ├── migrations/
│   └── templates/
│       └── index.html
└── env/
```

## Setup Instructions

1. **Clone the repository**
   ```sh
   git clone https://github.com/ChandraShekar00001/Mental-Health-Prediction-Using-Smartphone-Usage.git
   cd Mental-Health-Prediction-Using-Smartphone-Usage/mental_health_predictor
   ```

2. **Create and activate a virtual environment**
   ```sh
   python -m venv env
   .\env\Scripts\Activate.ps1   # For PowerShell
   ```

3. **Install dependencies**
   ```sh
   pip install -r requirements.txt
   ```
   If `requirements.txt` is missing, install manually:
   ```sh
   pip install django joblib scikit-learn numpy scipy
   ```

4. **Apply migrations**
   ```sh
   python manage.py migrate
   ```

5. **Run the development server**
   ```sh
   python manage.py runserver
   ```

6. **Access the app**
   Open [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in your browser.

## Usage

- Enter your smartphone usage details in the form.
- Click "Predict" to get your mental health prediction.

## License

This project is for educational purpose

