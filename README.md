Network Intrusion Detection System (NIDS)
Machine Learning-Based Cyber Attack Detection
A machine learning project that analyzes network traffic and classifies
it as BENIGN (normal traffic) or ATTACK (potentially malicious
traffic). The project uses the CIC-IDS2017 dataset and compares multiple
classification algorithms.

Project type: AIML / Machine Learning
Environment: Google Colab
Dataset: CIC-IDS2017
Project Overview
A Network Intrusion Detection System (NIDS) monitors network traffic and
identifies patterns that may indicate malicious activity. This project
trains machine learning models on labeled network traffic records and
predicts whether a record is benign or an attack.

Binary target encoding: - 0 --- BENIGN - 1 --- Any non-BENIGN attack
label
Objectives
- Analyze network traffic using a real dataset.
- Identify normal and malicious network activities.
- Apply and compare machine learning classifiers.
- Evaluate models using standard classification metrics.
- Identify important features and predict traffic classes.
Dataset
The project uses the CIC-IDS2017 dataset from the Canadian Institute for
Cybersecurity.
- Official dataset: https://www.unb.ca/cic/datasets/ids-2017.html
- Dataset mirror:
  https://huggingface.co/datasets/c01dsnap/CIC-IDS2017/tree/main
CSV files used: - Tuesday-WorkingHours.pcap_ISCX.csv -
Friday-WorkingHours-Afternoon-DDoS.pcap_ISCX.csv -
Friday-WorkingHours-Afternoon-PortScan.pcap_ISCX.csv
Technologies
Python, Google Colab, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn,
XGBoost, and Joblib.
Machine Learning Models
1. Logistic Regression
2. Decision Tree
3. Random Forest
4. XGBoost
Workflow
1. Load the CIC-IDS2017 CSV files.
2. Explore the dataset and class distribution.
3. Clean data and handle missing or infinite values.
4. Convert labels into BENIGN (0) and ATTACK (1).
5. Prepare features and target.
6. Perform a stratified 80:20 train-test split.
7. Train the four classification models.
8. Evaluate and compare model performance.
9. Review feature importance where supported.
10. Predict BENIGN or ATTACK for network traffic.
11. Save the trained model for future use.
Getting Started
Google Colab
1. Open https://colab.research.google.com/
2. Upload or open the project notebook.
3. Install XGBoost if required:
!pip install xgboost
4. Download the CSV files from the dataset source above.
5. Upload the files to Colab or place them in Google Drive.
6. Update the notebook paths to match your file locations.
7. Run the notebook cells in order.
Local Environment
Install the required packages:
pip install pandas numpy matplotlib seaborn scikit-learn xgboost joblib jupyter
Then run:
jupyter notebook
Dataset files are not included by default; download them separately.
Evaluation Metrics
- Accuracy: Overall percentage of correct predictions.
- Precision: How many predicted attacks are actually attacks.
- Recall: How many actual attacks were detected.
- F1-score: Harmonic mean of precision and recall.
- Confusion Matrix: Summarizes correct and incorrect predictions
  by class.
Recall and F1-score are important for intrusion detection, since missed
attacks can be costly and class distributions may be imbalanced.
Results
Run the notebook and fill in the actual metrics. Do not report estimated
or fabricated values.

  Model                   Accuracy   Precision   Recall   F1-score
  Logistic Regression          ---         ---      ---        ---
Decision Tree                ---         ---      ---        ---
Random Forest                ---         ---      ---        ---
XGBoost                      ---         ---      ---        ---

Best-performing model: Complete after comparing actual evaluation
results.
Suggested Repository Structure
Network-Intrusion-Detection-System/
├── Network_Intrusion_Detection.ipynb
├── README.md
├── requirements.txt
├── data/       # Download CIC-IDS2017 CSV files here
└── models/     # Saved model files, if generated
Limitations
- The model uses selected CIC-IDS2017 traffic files and may not
  generalize to all networks.
- Real network traffic can differ from the dataset.
- Data imbalance and data quality can affect performance.
- This is an academic demonstration, not a complete production
  security system.
Future Enhancements
- Include more CIC-IDS2017 traffic files.
- Extend to multiclass attack classification.
- Test on additional intrusion-detection datasets.
- Build a dashboard for predictions and evaluation.
- Explore real-time traffic analysis in a controlled environment.
- Improve detection of previously unseen attacks.
Conclusion
This project demonstrates how machine learning can support network
intrusion detection by learning patterns in network traffic and
classifying records as benign or potentially malicious. Comparing
multiple models provides a basis for selecting a suitable classifier and
further developing data-driven cybersecurity solutions.
Acknowledgements
- Canadian Institute for Cybersecurity, University of New Brunswick,
  for CIC-IDS2017.
- The open-source Python and machine learning communities.
