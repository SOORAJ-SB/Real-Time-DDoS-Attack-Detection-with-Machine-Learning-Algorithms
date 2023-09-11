
# Real-Time DDoS Attack Detection with Machine Learning Algorithms

## Overview

Welcome to the DDoS Attack Detection project, a cutting-edge system designed to identify and mitigate Distributed Denial of Service (DDoS) attacks using machine learning and Software-Defined Networking (SDN). This project aims to enhance network security by providing real-time detection of DDoS attacks, enabling timely response and mitigation measures.

## Key Features

- **Machine Learning-Based Detection:** Leveraging machine learning algorithms, including Decision Trees, this project offers robust DDoS attack detection by analyzing network traffic in real time.

- **SDN Integration:** The system is integrated into an SDN architecture, enhancing network flexibility and management while centralizing control.

- **Comprehensive Dataset:** We have generated a comprehensive dataset that includes both normal network traffic and various types of DDoS attack traffic (ICMP flood, UDP flood, TCP-SYN flood, and LAND attacks).

- **Model Training and Testing:** Different machine learning classifiers, such as K-Nearest Neighbors (KNN), Naïve Bayes (NB), Decision Tree (DT), and Random Forest (RF), were evaluated for training and testing. The Decision Tree classifier achieved the highest accuracy and was selected.

- **Real-Time Detection:** The trained model is deployed in real-time to detect and classify incoming network traffic as either benign or malicious, alerting administrators to potential DDoS attacks.

## How it Works

1. **Topology Setup:** The project utilizes two virtual machines - Mininet and Ryu Controller, each running Ubuntu (64 bit) with 4GB RAM. Mininet creates a network of virtual hosts, switches, controllers, and links, while Ryu Controller facilitates software-defined networking.

2. **Dataset Generation:** DDoS attack traffic is generated in Mininet, simulating ICMP, UDP, TCP-SYN, and LAND attacks. The Ryu Controller records the characteristics of both normal and attack traffic, creating a comprehensive dataset.

3. **Model Training:** Different classifiers are evaluated for their accuracy and training times. The Decision Tree classifier is chosen for its superior performance and is trained on the dataset.

4. **Real-Time Detection:** The trained model is deployed within the SDN architecture to monitor incoming network traffic in real time. It classifies traffic as benign or malicious and alerts administrators in the event of a potential DDoS attack.

## Getting Started

To get started with DDoS Attack Detection:

1. Clone this repository to your local machine.

2. Follow the setup instructions to configure the necessary dependencies and libraries, as detailed in the project's documentation.

3. Run the project, and explore the real-time detection capabilities by simulating DDoS attacks or analyzing normal traffic.

4. Review the project's accuracy results and analysis to gain insights into its performance.
