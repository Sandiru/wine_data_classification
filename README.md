# 🍷 Wine Classification using k-NN

This project uses the **Wine dataset** from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/) to build a classification model using the **k-Nearest Neighbors (k-NN)** algorithm. The objective is to classify wine types based on their chemical properties.

## 📦 Dependencies

To run the code, install the required Python packages:

```bash
pip install ucimlrepo pandas scikit-learn matplotlib
```

---

## 📂 Dataset

* **Source:** UCI Machine Learning Repository
* **Dataset ID:** 109 (Wine Dataset)
* **Features:** Various chemical properties of wine
* **Target:** Wine class (type 1, 2, or 3)

---

## 🔍 Feature Engineering

* Missing value check
* Feature scaling using:

  * `MinMaxScaler` for `Magnesium` and `Proline`
  * `StandardScaler` for selected features
* Feature selection using correlation threshold (`abs(correlation) >= 0.2`)

---

## 🧠 Model: k-Nearest Neighbors (k-NN)

* The dataset is split into training and test sets (70% training / 30% testing)
* Evaluated for k values from 1 to 40
* Accuracy scores are plotted to visualize the optimal `k`

---

## 📊 Results

* **Highest Accuracy:** 0.9815 (achieved at `k = 1` and `k = 3`)
* **Accuracy Range:** Mostly between 0.9444 to 0.9629
* As `k` increases, the accuracy becomes more stable but slightly lower

---

## 📈 Visualization

* A line graph is plotted for `Accuracy vs. Number of Neighbors (k)` using `matplotlib`

---

## ✅ Conclusion

The k-NN classifier performs very well on the Wine dataset, with the best results achieved at lower values of `k`. This project demonstrates essential steps in a machine learning pipeline, including data preprocessing, feature scaling, model training, evaluation, and visualization.

---


