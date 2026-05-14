# Customer Classification Category

## 📌 Introduction

This project was developed to build a Machine Learning system that can automatically classify customers into four different groups: A, B, C, and D based on their demographic and behavioral information. The purpose of this classification is to help businesses better understand their customers so they can create more effective marketing strategies, provide personalized services, and improve overall customer engagement.

---

# 📊 Dataset Information

The dataset used in this project contains **8,068 customer records** with **10 input features** and one target variable called **Segmentation**. Since the goal is to predict one out of four categories, the problem is considered a **multi-class classification task**.

### Feature Types

#### Quantitative Features
- Age
- Work_Experience
- Family_Size

#### Categorical Features
- Gender
- Ever_Married
- Graduated
- Profession
- Spending_Score
- Var_1

Categorical values were converted into numerical form using **Label Encoding**, as machine learning algorithms require numerical input for training and prediction.

Heatmap visualization were performed to better understand the dataset and identify relationships between features.

- Features such as **Age** and **Spending_Score** showed useful patterns related to customer segmentation.
- Most features remained relatively independent, which helped reduce redundancy in the dataset.
- The target classes were also reasonably balanced:
  - Segment A → 24.4%
  - Segment B → 23.0%
  - Segment C → 24.4%
  - Segment D → 28.1%

This balanced distribution helped the models learn more effectively during training.

---

## 📚 Libraries Used

### Core Libraries
- pandas – data manipulation and analysis  
- numpy – numerical computations  
- matplotlib – data visualization  
- seaborn – statistical data visualization  

### Scikit-learn Modules
- train_test_split – splitting dataset into training and testing sets  
- LabelEncoder – encoding categorical variables  
- StandardScaler – feature scaling  
- label_binarize – multi-class label processing  
- SimpleImputer – handling missing values  

### Evaluation Metrics
- accuracy_score  
- precision_score  
- recall_score  
- confusion_matrix  
- roc_curve  
- roc_auc_score  

### Machine Learning Models
- KNeighborsClassifier (KNN)  
- DecisionTreeClassifier  
- MLPClassifier (Neural Network)  
- KMeans (Clustering)

---

# 🤖 Model Performance

Several machine learning algorithms were tested during the project, and the **K-Nearest Neighbors (KNN)** model achieved the best overall performance. This indicates that customers within the same category tend to share very similar characteristics and feature patterns.

Feature scaling was one of the most important preprocessing steps because the performance of the KNN model dropped significantly without proper normalization.

---

# ⚠️ Challenges Faced

Some challenges encountered during the project included:

- Handling missing values in categorical columns such as **Profession**
- Managing a dataset with more categorical features than numerical features
- Ensuring proper feature scaling for better model performance
- Reducing possible bias caused by filling missing categorical values with the most frequent category

---

# 📌 Conclusion

Overall, the project successfully demonstrated how Machine Learning can be used to classify customers into meaningful groups using demographic and behavioral data. The results showed that customer-related information can effectively help businesses understand customer behavior and improve decision-making for marketing and customer engagement strategies.

---

# 👨‍💻 Authors

- Saad Noman Adeeb
- Mehreen Mallick Fiona
