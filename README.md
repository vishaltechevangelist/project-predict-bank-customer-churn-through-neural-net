# Bank Customer Churn Prediction using Artificial Neural Network (ANN)

## 📌 Project Description
This project aims to predict **bank customer churn** (whether a customer will leave the bank) using an **Artificial Neural Network (ANN)**.  
Customer churn is a major challenge for financial institutions, and predicting it in advance helps banks take proactive steps to retain valuable customers.  
The project demonstrates how deep learning can be applied to **tabular data** for classification tasks.  

---

## 📊 Dataset Details
The dataset used is the **Bank Customer Churn Dataset**, which typically contains demographic, account, and behavioral attributes of customers.  
Key features include:  
- **CustomerID** – Unique identifier (not used in modeling)  
- **Geography** – Country/region of customer  
- **Gender** – Male/Female  
- **Age** – Customer’s age  
- **Tenure** – Number of years the customer has stayed with the bank  
- **Balance** – Account balance  
- **NumOfProducts** – Number of products/services used  
- **HasCrCard** – Whether customer has a credit card (0/1)  
- **IsActiveMember** – Whether customer is active (0/1)  
- **EstimatedSalary** – Approximate annual salary  
- **Exited** – Target variable (1 = churn, 0 = retained)  

---

## 🛠️ Activities Performed
1. **Data Preprocessing**  
   - Handle missing values (if any)  
   - Encode categorical variables (Geography, Gender) using OneHotEncoding/LabelEncoding  
   - Feature scaling (StandardScaler/MinMaxScaler)  

2. **Model Development (ANN using Keras)**  
   - Define an ANN model with input, hidden, and output layers  
   - Use ReLU activation for hidden layers and Sigmoid for output layer  
   - Compile the model with `binary_crossentropy` loss and `adam` optimizer  

3. **Model Training & Evaluation**  
   - Split dataset into training and testing sets  
   - Train ANN and monitor performance using accuracy and loss metrics  
   - Evaluate the model on test data  

4. **Prediction**  
   - Generate predictions for customer churn probability  
   - Classify customers as “Churn” or “Retained”  

5. **Visualization & Insights**  
   - Plot training/validation accuracy and loss curves  
   - Summarize insights on key customer factors affecting churn  

---

✅ This project highlights the use of **deep learning on structured banking data** for customer retention strategies.  
README: Bank Customer Churn Prediction using ANN 🏦
Project Description
This project focuses on predicting customer churn for a bank using an Artificial Neural Network (ANN). Customer churn, or the loss of customers, is a significant challenge for businesses. By accurately predicting which customers are likely to leave, a bank can proactively take measures to retain them, such as offering special deals or improving services. This model leverages a deep learning approach to identify complex, non-linear patterns in customer data that traditional models might miss.

Dataset Details
The dataset used in this project is a CSV file named 'Churn_Modelling.csv'. It contains information about bank customers and includes 10,000 records across 14 features. The dataset is ideal for a supervised machine learning task, where the goal is to classify customers as either "churned" or "not churned."

Key features in the dataset include:

Customer-specific information: CustomerId, Surname

Demographics: CreditScore, Geography, Gender, Age

Account-specific data: Tenure (how long they've been a customer), Balance, NumOfProducts (number of bank products used), HasCrCard (whether they have a credit card), IsActiveMember (whether they are an active member)

Predictive features: EstimatedSalary

Target variable: Exited (1 if the customer churned, 0 otherwise)

Activities Performed
1. Data Preprocessing
Loading and inspection: The dataset was loaded using pandas. Initial checks were performed to understand its structure, identify missing values, and analyze the data types.

Feature engineering: Categorical features like 'Geography' and 'Gender' were converted into numerical formats using one-hot encoding to make them suitable for the ANN model. The Exited column was designated as the target variable.

Feature scaling: Numerical features were scaled using StandardScaler. This is a crucial step for ANNs as it helps the model converge faster and perform better by ensuring all features are on a similar scale.

2. Model Development
ANN architecture: A sequential model was built using Keras, a high-level API for TensorFlow. The network architecture consists of:

An input layer that matches the number of features.

Two hidden layers with a Rectified Linear Unit (ReLU) activation function.

An output layer with a sigmoid activation function, which is ideal for binary classification problems as it outputs a probability between 0 and 1.

Model compilation: The model was compiled with the Adam optimizer, which is an efficient optimization algorithm. The binary cross-entropy loss function was used, as it's the standard for binary classification, and the performance was monitored using accuracy as the metric.

3. Training and Evaluation
Splitting data: The dataset was split into training and testing sets to evaluate the model's performance on unseen data.

Model training: The ANN was trained on the training data for a specified number of epochs with a defined batch size.

Model evaluation: The trained model's performance was evaluated on the test set using various metrics, including accuracy, precision, recall, and the F1-score, providing a comprehensive view of its predictive power.
