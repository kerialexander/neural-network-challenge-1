# Student Loan Repayment Prediction - Neural Network Challenge
Module 18 Challenge Assignment - Neural Network Challenge

# Project Overview
This project focuses on developing a neural network model to predict student loan repayment likelihood, enabling more accurate interest rates for borrowers. By analyzing data on past student loan recipients, such as credit ranking, academic performance, and financial history, the model aims to predict credit quality and repayment success.  

The project is divided into four key parts:
1. **Data Preparation:** The dataset is preprocessed by creating feature and target sets, scaling the data, and splitting it into training and testing subsets.  
2. **Model Development:** A deep neural network is built using TensorFlow and Keras, with layers and neurons configured to reflect the complexity of the input data. The model is compiled with the binary cross-entropy loss function and evaluated for accuracy.  
3. **Prediction and Evaluation:** The trained model is used to predict repayment success, and results are validated through classification reports.  
4. **Recommendation System:** A context-based filtering approach is proposed to recommend student loan options, leveraging academic, financial, and behavioral data.  

This solution helps identify high-risk borrowers and tailor loan offerings, contributing to responsible lending practices. 

## Model Development Environment  

The student loan repayment prediction model was created using **Python** in a **Jupyter Notebook** on **Google Colab**.  

### Key Tools and Libraries:  
- **Python** – Core programming language for data manipulation, machine learning, and neural network development.  
- **Pandas** – Used for data loading, cleaning, and preprocessing.  
- **Scikit-Learn** – Employed for data scaling, train-test splitting, and evaluating model performance.  
- **TensorFlow/Keras** – Utilized to build, compile, and train the deep neural network for predicting loan repayment.  
- **Matplotlib** – Applied for visualizing data correlations and insights.  

### Development Process:  
- The project was initially started by uploading the dataset and Jupyter Notebook to Google Colab.  
- All code was developed and executed in Colab to leverage its GPU capabilities and cloud environment.  
- The trained model was saved and exported as a **Keras** file for deployment and further testing.  

Using Google Colab provided the advantage of scalable computing resources, making it easier to handle data preprocessing and neural network training efficiently.  

## Analysis

### Correlation Analysis
A correlation matrix was generated to analyze the relationships between key variables in the dataset. Key findings include:  
- **Positive Correlations:**  
  - *Payment History & STEM Degree Score (0.67):* Students pursuing STEM degrees tend to have stronger repayment histories, indicating lower risk.  
  - *Finance Workshop Score & Payment History (0.67):* Financial literacy is linked to better repayment behavior, suggesting that students with financial education are more responsible borrowers.  
  - *Alumni Success & Total Loan Score (0.37):* Institutions with successful alumni correlate with higher loan scores, reflecting greater earning potential.  

- **Negative Correlations:**  
  - *Cohort Ranking & Payment History (-0.68):* Lower cohort rankings align with better payment history, indicating higher-achieving students are more financially responsible.  
  - *Location Parameter & STEM Degree (-0.55):* Regional differences impact the likelihood of pursuing STEM degrees, affecting overall repayment risk.  

### Model Performance
A Random Forest Regressor was used to predict loan scores, yielding the following results:  
- **Mean Squared Error (MSE):** 0.0111 – Reflects low prediction error.  
- **R² Score:** 0.487 – The model explains approximately 48.7% of the variance in loan scores, suggesting moderate predictive accuracy.  

### Key Insights
- **Financial Literacy is Crucial:** Strong correlations between financial workshop scores and repayment history indicate that incorporating financial literacy training could reduce loan defaults.  
- **STEM Students are Lower Risk:** Students in STEM fields consistently show better repayment behavior, making them prime candidates for favorable loan terms.  
- **Dynamic Data is Essential:** The model’s moderate performance highlights the need to incorporate more dynamic, real-time data to improve accuracy.  

Future improvements could involve refining the model architecture, incorporating additional financial indicators, and using advanced neural networks to enhance performance.  

## Summary Questions

### 1. Data for Student Loan Recommendation System
To build a student loan recommendation system, key data points include academic performance (GPA, degree type, major), financial background (family income, credit score, financial aid eligibility), and behavioral indicators (payment history, financial literacy). This data is relevant because it reflects a student's ability to manage debt, predicts future earning potential, and ensures personalized loan recommendations that align with individual financial needs and repayment capacity.

### 2. Filtering Method for Recommendation System
The model would use **context-based filtering** because the recommendation is driven by individual attributes such as financial background, academic performance, and creditworthiness. This approach tailors recommendations based on a student's personal data, unlike collaborative filtering, which relies on group behavior patterns. Context-based filtering ensures that loan options are aligned with each student's unique profile, making the recommendations more relevant and accurate.

### 3. Real-World Challenges in Building the System
- **Data Privacy:** Sensitive data like credit scores and family income must be protected to ensure compliance with regulations and maintain user trust. Any breach could discourage students from using the system.  
- **Financial Unpredictability:** Students' financial situations can change, making static data unreliable over time. A system that adapts to real-time updates can better reflect current needs and offer appropriate loan recommendations.  

Addressing these challenges ensures that the recommendation system remains secure, accurate, and capable of evolving with the user's financial journey.  

## Real-World Challenges

Building a student loan recommendation system presents several real-world challenges that must be addressed to ensure accuracy, fairness, and user trust.  

### 1. Data Privacy and Security  
- **Challenge:** The system relies on sensitive information such as credit scores, family income, and academic records. This data must be securely stored and transmitted to comply with privacy regulations (e.g., FERPA, GDPR).  
- **Concern:** A breach or unauthorized access to this information could lead to identity theft, loss of trust, and legal repercussions. Ensuring data encryption, user consent, and strict access controls is vital to protect users and maintain the system’s integrity.  

### 2. Financial Unpredictability  
- **Challenge:** A student’s financial situation can change rapidly due to unexpected life events, economic downturns, or family emergencies.  
- **Concern:** Loan recommendations based on static or outdated data may no longer reflect the student's actual financial capacity, resulting in unsuitable loan offers. By incorporating real-time data updates and flexible models, the system can adapt to changes, providing more relevant and personalized recommendations.  

### 3. Bias in Loan Recommendations  
- **Challenge:** The use of historical data may inadvertently introduce biases, leading to unequal loan offers for certain groups of students.  
- **Concern:** If not addressed, this could perpetuate inequalities in lending. Regular audits, diverse datasets, and fairness constraints in the model can help mitigate bias and ensure equitable loan recommendations for all users.  

### 4. Limited Credit History for Students  
- **Challenge:** Many students have limited or no credit history, making it difficult to assess their repayment ability.  
- **Concern:** This lack of data may result in conservative loan offers or high-interest rates. Incorporating alternative indicators like academic performance, participation in financial literacy programs, and co-signer data can help address this gap and provide better loan options.  

Addressing these challenges enhances the reliability and fairness of the student loan recommendation system, ultimately benefiting both lenders and students.  

# Resources 
I also attended a tutoring session to review the code I had written and reviewed a warning message the code produced to better understand what could have been done differently.
