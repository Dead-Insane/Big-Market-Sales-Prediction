# 🛒 Big Market Sales Prediction

## 📊 Overview
This project aims to **predict the sales of various products in different Big Mart outlets**.  
By analyzing a dataset of product and outlet information, we build a **machine learning model** to forecast future sales, which can help in **strategic business planning and inventory management**.  

The project follows a standard data science workflow, including **exploratory data analysis (EDA)**, **data preprocessing**, and **model training & evaluation**.  

---

## 📁 Project Structure
notebooks/ # Jupyter Notebook (.ipynb) files
data/ # Raw dataset (bigmarket.csv)
README.md # Project documentation
---

## 🛠️ Key Steps

### 🔍 Exploratory Data Analysis (EDA)
**Objective:** Understand dataset characteristics, detect patterns, and find missing values or anomalies.  
**Key Activities:**
- Visualizing numerical features using **distribution plots** (`displot`).  
- Analyzing categorical features with **count plots** (`countplot`).  
- Identifying key factors influencing product sales.  

---

### 🧹 Data Preprocessing
**Objective:** Clean and transform raw data into a suitable format for ML models.  
**Key Activities:**
- Handling missing values (e.g., `Item_Weight`, `Outlet_Size`).  
- Applying **Label Encoding** to categorical features (e.g., `Outlet_Location_Type`).  
- Fixing inconsistencies in categorical data (e.g., `Item_Fat_Content`).  

---

### 🤖 Model Building & Evaluation
**Objective:** Train predictive models and evaluate performance.  
**Key Activities:**
- **Splitting Data**: Features (`X`) vs target (`y = Item_Outlet_Sales`).  
- **Train-Test Split**: Evaluate performance on unseen data.  
- **Model Training**: Implemented with **TensorFlow/Keras** regression models.  
- **Evaluation Metrics**: Used **Root Mean Squared Error (RMSE)** to assess performance.  

---

## 🚀 How to Run the Project

### 1. Clone the Repository
```bash
git clone https://github.com/Dead-Insane/Big-Market-Sales-Prediction.git
cd Big-Market-Sales-Prediction
```
### 2. Set up the Enviroment
```bash
conda create -n bigmart python=3.10 -y
conda activate bigmart
conda install jupyter tensorflow numpy pandas scikit-learn matplotlib seaborn -y
```
### 3. Run Jupyter Notebook
```bash
jupyter notebook notebooks/big-market-sales-prediction.ipynb
```
### 4. Results
- The trained model provides a strong foundation for sales prediction, achieving a relatively low **Root Mean Squared Error (RMSE)** on the test data.  
- This indicates that the model's predictions are, on average, close to the actual sales values.  
- The insights from the **EDA** and the performance of the model demonstrate the viability of this approach for **forecasting**.  

---

## 🔮 Future Work
- **Hyperparameter Tuning**: Optimize the model's performance by tuning hyperparameters of the TensorFlow/Keras algorithm.  
- **Alternative Models**: Explore other machine learning algorithms, such as Gradient Boosting or Random Forest, to see if they yield better results.  
- **Feature Engineering**: Create new features from the existing data to improve the model's predictive power.  
- **Data Acquisition**: Integrate additional data sources, such as economic indicators or local events, to enhance forecasting accuracy.  

---
