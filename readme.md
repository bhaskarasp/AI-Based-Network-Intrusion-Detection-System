# AI-Powered Network Intrusion Detection System (NIDS)

Welcome to the AI-powered Network Intrusion Detection System (NIDS) project. This application uses machine learning to analyze network traffic and classify it into two categories:

### Benign (Safe): Normal network traffic.

### Malicious (Attack): Potential cyberattacks such as DDoS, port scans, and other forms of network intrusions.

## Features:

### Real-Time Traffic Classification: Classify network traffic based on simulated packet data.

### Interactive Streamlit Dashboard: Easily train and evaluate the model with visualized metrics and real-time testing.

### Performance Metrics: Get the model's performance metrics, such as accuracy, confusion matrix, and detected threats.

### Live Traffic Simulator: Test custom network traffic inputs to see if the system flags them as malicious or benign.

## Technologies Used:

### Streamlit: Framework for building the interactive dashboard.

### Scikit-learn: For machine learning model (Random Forest).

### Seaborn & Matplotlib: For data visualization (confusion matrix).

### Pandas & Numpy: For data handling and simulation.

## Installation & Setup
1. Clone the Repository:
git clone https://github.com/yourusername/nids.git
cd nids

2. Install Dependencies:

Make sure you have Python 3.x installed, then run:

pip install -r requirements.txt

3. Running the Application:

Once dependencies are installed, run the Streamlit app with the following command:

streamlit run app.py


The application will start locally on your browser (usually at http://localhost:8501).

## How to Use the Application:

### Train the Model:

Adjust the training data split and number of trees using the sidebar controls.

Click the "Train Model Now" button to start training the Random Forest classifier.

### Evaluate Model Performance:

After training, you can view the accuracy, confusion matrix, and detected threats.

### Test Live Traffic Simulation:

Input custom network traffic parameters (flow duration, packet count, etc.) in the Live Traffic Simulator section.

Click "Analyze Packet" to see if the system flags it as an attack or benign traffic.

Example Output:

Accuracy: 97.56%

Total Samples: 5000

Detected Threats: 150

Confusion Matrix Visualization:

### Future Improvements:

Integrate a real-world network traffic dataset (e.g., CIC-IDS2017).

Enhance the UI for more interactive feedback.

Implement additional machine learning models for comparison.

Add logging and alerting for real-time network monitoring.

## License:

This project is licensed under the MIT License - see the LICENSE
 file for details.

## requirements.txt

Make sure to include the necessary dependencies in the requirements.txt for easy installation:

streamlit==1.10.0
pandas==1.4.2
numpy==1.22.4
scikit-learn==0.24.2
seaborn==0.11.2
matplotlib==3.5.1