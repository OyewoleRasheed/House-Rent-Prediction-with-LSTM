# 🏡 House Rent Prediction Using LSTM (Deep Learning)

This project predicts **house rental prices** using a **deep learning model with LSTM (Long Short-Term Memory)** networks.  
It leverages past house rent trends to forecast future rent prices more accurately.

🔗 **Original Tutorial:** [House Rent Prediction with Machine Learning – The Clever Programmer](https://thecleverprogrammer.com/2022/08/15/house-rent-prediction-with-machine-learning/)

---

## 📂 Dataset Overview

The dataset contains historical house rental price information, including:

- **Size** (area in square feet)
- **Number of Bedrooms (BHK)**
- **Floor Number**
- **Area Type**
- **City**
- **Furnishing Status**
- **Tenant Preferred**
- **Number of Bathrooms**
- **Rent Price** (target variable)

---

## 🛠️ Technologies Used

- **Python** 🐍
- **NumPy**, **Pandas** for data manipulation
- **Matplotlib**, **Seaborn** for data visualization
- **TensorFlow** and **Keras** for building the LSTM model
- **Scikit-learn** for preprocessing and metrics
- **Jupyter Notebook** for interactive development

---

## 🚀 Workflow

1. **Data Cleaning & Preprocessing**:
   - Dropped irrelevant columns like "Posted On."
   - Encoded categorical variables (e.g., Area Type, Furnishing Status, Tenant Type).
   - Normalized rent values using MinMaxScaler.
   - Prepared sequences for LSTM model input.

2. **Data Splitting**:
   - Split the data into training and testing sets (80%-20%).

3. **Model Building**:
   - Designed an LSTM-based Sequential model:
     - 1st LSTM layer (128 units, return sequences=True)
     - 2nd LSTM layer (64 units, return sequences=False)
     - Dense layer (25 neurons)
     - Output Dense layer (1 neuron)
   - Used **Mean Squared Error (MSE)** as the loss function.
   - Optimized using **Adam** optimizer.

4. **Training**:
   - Trained the model for a number of epochs (commonly 20-30) to minimize loss.

5. **Evaluation**:
   - Predicted house rent prices on the test set.

---

## 📈 Results

- Successfully built a working **LSTM model** that predicts house rental prices based on historical trends.
- Visualization showed that the model could capture rental price patterns reasonably well.

---

## 🧠 Key Learnings

- How to use **LSTM networks** for sequence modeling problems like rent prediction.
- Data preprocessing and sequence creation for LSTM input.
- Importance of scaling data when training deep learning models.
- Visualizing model performance with real vs predicted curves.

---

## 📌 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/OyewoleRasheed/House-Rent-Prediction-with-LSTM
   cd House-Rent-Prediction-with-LSTM
   ```

2. Install the dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn tensorflow
   ```

3. Launch the Jupyter Notebook:
   ```bash
   jupyter notebook house_rent_Prediction.ipynb
   ```

---

## 🤝 Acknowledgments

Thanks to **The Clever Programmer** for the project inspiration and walkthrough.

---

# 📬 Contact
**GitHub**: [https://github.com/OyewoleRasheed]  
**LinkedIn**: [https://www.linkedin.com/in/rasheed-adebayo-oyewole-gmnse-815333184/]  
Feel free to connect!

---
