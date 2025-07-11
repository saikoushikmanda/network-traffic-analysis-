# network-traffic-analysis-
This project uses machine learning to classify and analyze network traffic data. It helps in identifying different types of traffic (e.g., benign or malicious) and detecting anomalies using algorithms such as Random Forest and Isolation Forest.
As network threats continue to grow in complexity, automated approaches to traffic classification and anomaly detection are becoming essential. This project demonstrates how supervised and unsupervised machine learning algorithms — including Random Forest and Isolation Forest — can be applied to network traffic logs to detect potential attacks like DoS, Port Scanning, or unknown anomalies.

**Features**
Upload and process CSV-based network traffic datasets

Data preprocessing: drop irrelevant columns, handle missing values, normalize features

Train and evaluate a Random Forest Classifier

Apply Isolation Forest for unsupervised anomaly detection

Optimize model performance using Grid Search (GridSearchCV)

Display classification reports and sample anomaly detection output

Fully implemented in Python and compatible with Jupyter or Google Colab

 **Getting Started**
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/network-traffic-ml.git
cd network-traffic-ml
2. Install Dependencies
bash
Copy
Edit
pip install pandas scikit-learn
3. Run the Notebook
Open 1-network traffic.ipynb using Jupyter or upload it to Google Colab.

4. Upload Dataset
Use your own .csv file or the provided extended_network_traffic.csv. Make sure it includes:

Numerical features

A Label column (e.g., Benign, DoS, etc.)

**How It Works**
**1.Upload CSV**
File is loaded using pandas.read_csv() and previewed.

**2.Preprocessing**
Drops IPs, timestamps, and other non-numeric fields. Scales data using StandardScaler.

**3.Model Training**
Trains a Random Forest classifier on 80% of the data, tests on 20%.

**4.Anomaly Detection**
Trains an Isolation Forest on benign traffic, flags anomalies in test data.

**5.Model Optimization**
Uses Grid Search to find the best hyperparameters for the classifier.

