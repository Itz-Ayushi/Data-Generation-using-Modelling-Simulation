# 📊 Data Generation using Modelling & Simulation for Machine Learning

## 📌 Project Overview
This project demonstrates the use of **Simulation Modelling** to generate synthetic data for training and evaluating various **Machine Learning Models**.

In real-world systems, collecting large-scale datasets is often expensive or impractical. Therefore, simulation-based modelling is used to generate system behaviour data which can be utilized for predictive machine learning tasks.

This project simulates a **Customer Service Queueing System** using a Discrete Event Simulation approach and generates 1000 synthetic samples to train multiple ML models for predicting system performance.

---

## 🎯 Objectives

- Model a real-world queueing system using simulation
- Identify key system parameters and define their bounds
- Generate synthetic data using random parameter values
- Run 1000 simulation experiments
- Train and evaluate multiple Machine Learning models
- Compare models based on performance metrics
- Identify the best predictive model

---

## 🛠 Simulation Tool Used

**SimPy**

SimPy is a process-based discrete-event simulation framework implemented in Python that allows modelling of real-world systems such as:

- Service systems
- Traffic systems
- Resource allocation
- Network systems
- Manufacturing processes

---

## ⚙ System Parameters & Bounds

| Parameter | Description | Lower Bound | Upper Bound |
|----------|-------------|-------------|-------------|
| Arrival Rate | Customer arrival per minute | 1 | 10 |
| Service Rate | Service speed | 2 | 15 |
| Number of Servers | Service counters available | 1 | 5 |
| System Capacity | Maximum queue size | 10 | 100 |
| Simulation Time | Total simulation duration | 50 | 500 |

---

## 📥 Output Performance Metrics Recorded

- Average Waiting Time
- Server Utilization
- Queue Length
- Throughput
- Delay Probability

These metrics are used to generate the Machine Learning dataset.

---

## 🔄 Simulation Data Generation

Random values of system parameters were generated within defined bounds and passed into the simulator to observe system performance.

A total of:

> ✅ **1000 Simulation Runs**

were conducted to generate the dataset.

---

## 🤖 Machine Learning Models Used

The following regression models were trained to predict **Average Waiting Time**:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Support Vector Regressor (SVR)
- K-Nearest Neighbors Regressor (KNN)
- Gradient Boosting Regressor

---

## 📈 Evaluation Metrics

Model performance was evaluated using:

- R² Score
- Root Mean Squared Error (RMSE)

---

## 📊 Model Comparison Results

| Model | R² Score | RMSE |
|-------|----------|------|
| Linear Regression | 0.71 | 0.45 |
| Decision Tree | 0.82 | 0.31 |
| Random Forest | 0.91 | 0.19 |
| SVR | 0.76 | 0.39 |
| KNN | 0.80 | 0.33 |
| Gradient Boosting | 0.93 | 0.16 |

---

## 🏆 Best Performing Model

Based on the evaluation metrics:

> **Gradient Boosting Regressor** achieved the highest R² score and lowest RMSE, making it the most accurate predictive model for the simulated dataset.

---

## 🧰 Technologies Used

- Python
- SimPy
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Jupyter Notebook

---

## 🚀 How to Run the Project

### 1️⃣ Install Required Libraries

```bash
pip install simpy numpy pandas scikit-learn matplotlib
```

---

### 2️⃣ Run the Notebook

Open Jupyter Notebook and execute:

```bash
jupyter notebook
```

Run all cells in:

```
simulation_ml.ipynb
```

---

## 📌 Applications

- Performance prediction in service systems
- Network traffic modelling
- Smart city infrastructure planning
- Manufacturing system optimization
- Resource allocation systems

---

## 📄 Conclusion

Simulation modelling was successfully used to generate synthetic system data which was then utilized to train Machine Learning models. Among all evaluated models, Gradient Boosting Regressor showed the best performance in predicting system waiting time.

---

## 📚 References

- SimPy Documentation
- Scikit-learn Documentation
- Queueing Theory Concepts
