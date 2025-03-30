# Customer Churn Prediction Web Application

This is a Flask web application that predicts customer churn probability based on various customer attributes.

## Features
- Web interface for inputting customer data
- Real-time churn prediction
- Probability-based classification

## Deployment Instructions

### Deploying to Render.com

1. Create a new account on [Render.com](https://render.com)
2. Click "New +" and select "Web Service"
3. Connect your GitHub repository
4. Configure the deployment:
   - Name: Choose a name for your service
   - Environment: Python
   - Build Command: `pip install -r requirements.txt`
   - Start Command: `gunicorn app:app`
   - Plan: Free

### Local Development

1. Clone the repository
2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the application:
   ```bash
   python app.py
   ```

## Project Structure
- `app.py`: Main Flask application
- `templates/`: HTML templates
- `static/`: Static assets
- `models/`: Trained model and column definitions
- `requirements.txt`: Project dependencies
- `Procfile`: Deployment configuration 