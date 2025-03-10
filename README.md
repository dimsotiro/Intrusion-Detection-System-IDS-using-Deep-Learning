# Intrusion-Detection-System-IDS-using-Deep-Learning
1) This repository contains a Deep Learning-based Intrusion Detection System (IDS) built using TensorFlow and Keras. The system is designed to detect cyber intrusions based on network traffic and user behavior.

The dataset used for this project comes from Kaggle(https://www.kaggle.com/datasets/dnkumars/cybersecurity-intrusion-detection-dataset), which contains network-based and user behavior-based features to classify activity as either normal or an attack.

2) Features
Network-Based Features

network_packet_size: Packet size (bytes); abnormal sizes may indicate attacks.
protocol_type: Protocol used (TCP, UDP, ICMP); certain attacks exploit specific protocols.
encryption_used: AES, DES, or None; weak encryption can be a vulnerability.

User Behavior-Based Features

login_attempts: Repeated logins may indicate brute-force attacks.
session_duration: Long sessions may indicate unauthorized persistence.
failed_logins: High values suggest credential stuffing attempts.
unusual_time_access: A binary flag for suspicious login times.
ip_reputation_score: Score from 0 to 1; higher values indicate suspicious activity.
Target Variable

attack_detected: 1 = Attack, 0 = Normal Activity

3) Prerequisites
Ensure you have the following installed:
Python 3.x
TensorFlow
NumPy
Pandas
Matplotlib

4) Training the Model
Training involves:
Batch size: 100
Epochs: 100 (Early Stopping enabled)
Training Split : 10% of data
Validation Split: 10% of data
Test Split : Training Split - Validation Split
5) Results
Training Accuracy: ~86.6%
Validation Accuracy: ~85.5%
Test Accuracy: ~84.3%
Loss Comparison: Training and validation losses are close, indicating minimal overfitting.
6) Contributors
Dimitris Sotiropoulos
Feel free to contribute by submitting issues or pull requests!
7) License
This project is open-source under the MIT License.
