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

---

✅ This project highlights the use of **deep learning on structured banking data** for customer retention strategies.  
