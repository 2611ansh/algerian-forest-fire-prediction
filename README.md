# Algerian Forest Fire Prediction

This is the README file for the "Algerian Forest Fire Prediction" project. This project aims to predict forest fire occurrences in Algeria based on various environmental factors. The prediction model is implemented in a Flask web application, allowing users to input environmental data and get predictions for forest fire likelihood.

## Project Structure

The project consists of the following components:

- `application.py`: This is the main Python file containing the Flask web application. It loads a pre-trained Ridge Regression model and a Standard Scaler for data preprocessing.

## Getting Started

To run the project locally, follow these steps:

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/2611ansh/algerian-forest-fire-prediction.git
   ```

2. Navigate to the project directory:

   ```bash
   cd algerian-forest-fire-prediction
   ```

3. Install the required Python packages. It's recommended to use a virtual environment:

   ```bash
   pip install -r requirements.txt
   ```

4. Run the Flask application:

   ```bash
   python application.py
   ```

   The application will be accessible at [http://localhost:5000](http://localhost:5000) in your web browser.

## Usage

Once the application is running, you can access it through your web browser. The following routes are available:

- `/`: The home page of the application, where you can enter data for prediction.
- `/predictdata`: The endpoint for predicting forest fire likelihood based on input data.

## Input Data

To make a prediction, enter the following environmental data on the `/` page:

- Temperature
- Relative Humidity (RH)
- Wind Speed (Ws)
- Rainfall (Rain)
- Fine Fuel Moisture Code (FFMC)
- Duff Moisture Code (DMC)
- Initial Spread Index (ISI)
- Classes (fire classes)
- Region

## Prediction

After entering the required data, click the "Predict" button. The application will use the trained model to predict the likelihood of a forest fire, and the result will be displayed on the home page.

## Model and Data Preprocessing

The project uses a Ridge Regression model for prediction. The model is loaded from the `models/ridge.pkl` file, and data preprocessing is performed using a Standard Scaler loaded from the `models/scaler.pkl` file.

## Acknowledgments

- The Algerian forest fire dataset used for training and testing the model.
- Flask for creating the web application.
- Scikit-learn for machine learning functionalities.
- The open-source community for valuable resources and inspiration.

Feel free to reach out for any questions or suggestions related to this project. Happy predicting!
