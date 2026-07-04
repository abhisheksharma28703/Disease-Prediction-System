# Multiple Disease Prediction System

* Machine learning based web app to predict multiple diseases based on user input data.
* Web app hosted on Streamlit with multiple pages. Each page takes input for a particular disease, and that data is fed to the model trained specifically for that disease.
* Used three different datasets to train three ML models — Support Vector Machine, Logistic Regression, and Random Forest — for predicting diabetes, heart disease, and Parkinson's disease respectively, and deployed them using pickle.
* **Exposure:** Streamlit, SVM, Logistic Regression, Random Forest, Scikit-learn, Pandas, NumPy.

🔗 **Live App:** [disease-prediction-system-rdxecxwyccdodd7hutzydw.streamlit.app](https://disease-prediction-system-rdxecxwyccdodd7hutzydw.streamlit.app)

---

# Logistic Regression

* Logistic Regression is a classification algorithm used to predict the probability that a given input belongs to a particular class.
* Instead of fitting a straight line like linear regression, it passes the weighted sum of input features through a sigmoid function, which squeezes any real-valued number into a range between 0 and 1 — this output is interpreted as a probability.
* A threshold (commonly 0.5) is then applied to this probability to assign the final class label. In this project, Logistic Regression is used for the **Heart Disease Prediction** model, where it estimates the probability of a patient having heart disease based on 13 clinical parameters.

<img width="607" height="485" alt="Logistic_regression" src="https://github.com/user-attachments/assets/ea4beab6-b3ac-4bd5-9562-cc6a04fc1dae" />


---

# SVM (Support Vector Machine)

* SVM is a robust classification algorithm that works by finding the optimal hyperplane that best separates data points belonging to different classes.
* It maximizes the margin — the distance between the hyperplane and the nearest data points from each class, known as support vectors — which helps the model generalize well to unseen data.
* For datasets that aren't linearly separable, SVM uses the kernel trick (e.g., RBF, polynomial) to project data into a higher-dimensional space where a clean separation becomes possible. In this project, SVM is used for the **Diabetes Prediction** model.

<img width="600" height="400" alt="SVM" src="https://github.com/user-attachments/assets/c7381062-7d5a-474d-b340-7dd6b477b4b3" />


---

# Random Forest

* Random Forest is an ensemble learning algorithm that builds multiple decision trees during training and combines their outputs to make a final, more reliable prediction.
* Each tree is trained on a random subset of the data and a random subset of features, which introduces diversity among the trees and reduces the risk of overfitting compared to a single decision tree.
* The final prediction is typically obtained through majority voting across all trees. In this project, Random Forest is used for the **Parkinson's Disease Prediction** model, which analyzes 22 biomedical voice measurements.

<img width="1500" height="898" alt="Random Forest" src="https://github.com/user-attachments/assets/1facd59f-6635-4d5e-bf11-fef71d133904" />


---

# Working Web App

* Enter the required medical parameters on the relevant page to get an instant prediction.

### Diabetes Prediction
<img width="1911" height="963" alt="Working Web App" src="https://github.com/user-attachments/assets/5c9860e4-d3f1-4eaf-ba6d-931d8b14fdd1" />


### Heart Disease Prediction
<img width="1918" height="968" alt="HeartDisease" src="https://github.com/user-attachments/assets/beaba6d3-718c-412c-88da-5cb6e45b1bc5" />


### Parkinson's Disease Prediction
<img width="1907" height="965" alt="Parkinsons Disease" src="https://github.com/user-attachments/assets/d654fc52-02ce-4960-82cb-fff50dbf4c03" />


---

# Tech Stack

- **Frontend/Deployment:** Streamlit, Streamlit Option Menu
- **ML & Data Processing:** Scikit-learn, NumPy, Pandas
- **Model Persistence:** Pickle
- **Language:** Python

---

# Running Locally

```bash
git clone https://github.com/abhisheksharma28703/Disease-Prediction-System.git
cd Disease-Prediction-System

python -m venv venv
venv\Scripts\activate      # Windows
source venv/bin/activate   # macOS/Linux

pip install -r requirements.txt
streamlit run app.py
```

---

# Future Works

* More types of diseases can be added for prediction.
* Better/ensemble models can be experimented with to achieve higher accuracy.
* Add model confidence scores alongside binary predictions.

---

# Author

**Abhishek Sharma**
Final-year B.Tech student, IIT (BHU) Varanasi
