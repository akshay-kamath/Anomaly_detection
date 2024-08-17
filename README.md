# Anomaly Detection System

## Overview

This project is an anomaly detection system that utilizes a Flask backend to process CSV data and detect anomalies using machine learning algorithms. The frontend is built with React to provide an interactive user experience for uploading files and visualizing results.

## Features

- **Upload and Process CSV Files:** Upload CSV files via a Flask API.
- **Anomaly Detection:** Detect anomalies using the Isolation Forest algorithm.
- **Data Visualization:** Visualize anomalies with decision boundary plots.
- **Summary and Insights:** Generate summaries and insights based on detected anomalies.

## Frontend

The frontend is implemented using React. It allows users to upload CSV files and view the results returned by the Flask API.

## Backend

The backend is implemented using Flask and includes the following features:

- **CSV Upload Endpoint:** `/api/uploadfile` - Accepts a POST request with a CSV file for anomaly detection.
- **Anomaly Detection:** Utilizes the Isolation Forest algorithm to identify anomalies.
- **Plotting:** Generates and returns base64-encoded plots of detected anomalies.
- **Summary and Insights:** Provides textual summaries and insights based on the anomaly detection results.

## Installation

### Backend

1. **Clone the repository:**

    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2. **Create a virtual environment and install dependencies:**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    pip install -r requirements.txt
    ```

3. **Run the Flask app:**

    ```bash
    python app.py
    ```

### Frontend

1. **Navigate to the frontend directory:**

    ```bash
    cd <frontend-directory>
    ```

2. **Install dependencies:**

    ```bash
    npm install
    ```

3. **Run the React app:**

    ```bash
    npm start
    ```

## How to Use

1. **Frontend:**

   - Place your CSV files in the designated upload area on the React app.
   - Submit the files to the Flask backend using the provided upload functionality.
   - View the results, including summaries, insights, and visualizations.

2. **Backend:**

   - **Upload your CSV file** through the API endpoint `/api/uploadfile`.
   - The backend will process the file, detect anomalies, and return results including:
     - Anomalies in JSON format.
     - A summary of the dataset and detected anomalies.
     - Insights based on the detected anomalies.
     - Base64-encoded plots for visualization.

## Libraries and APIs Used

- **Flask**: For building the backend API.
- **Pandas**: For data manipulation and analysis.
- **Matplotlib**: For generating plots.
- **Scikit-Learn**: For implementing the Isolation Forest algorithm.
- **Flask-CORS**: For handling Cross-Origin Resource Sharing.
- **React**: For building the frontend application.

## Credits

This project was developed by [Your Name](https://github.com/your-github-profile).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

