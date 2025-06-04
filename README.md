# ai-ml_Intern-Task-6
#  K-Nearest Neighbors (KNN) Classification on Iris Dataset

## 📌 Objective
Implement and understand the K-Nearest Neighbors (KNN) algorithm for multi-class classification using the classic **Iris** dataset. Evaluate the performance, experiment with different values of `K`, and visualize decision boundaries for model interpretability.

---

## 🛠️ Tools & Libraries
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## 📂 Dataset
- **Name**: Iris Flower Dataset
- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/iris)
- **Features**:
  - SepalLengthCm
  - SepalWidthCm
  - PetalLengthCm
  - PetalWidthCm
- **Target**: Species (Setosa, Versicolor, Virginica)
-  Id  SepalLengthCm  SepalWidthCm  PetalLengthCm  PetalWidthCm      Species
0   1            5.1           3.5            1.4           0.2  Iris-setosa
1   2            4.9           3.0            1.4           0.2  Iris-setosa
2   3            4.7           3.2            1.3           0.2  Iris-setosa
3   4            4.6           3.1            1.5           0.2  Iris-setosa
4   5            5.0           3.6            1.4           0.2  Iris-setosa

---

## 🔍 Steps Performed

1. **Loaded and explored the dataset** using `pandas`.
2. **Preprocessed** the data:
   - Dropped unnecessary columns (`Id`)
   - Encoded target labels using `LabelEncoder`
   - Normalized features using `StandardScaler`
3. **Split** the data into training and test sets (70/30 split).
4. **Trained KNN** classifier for different values of `K` (1 to 10).
5. **Evaluated accuracy** and selected the best `K` using accuracy score.
6. **Plotted confusion matrix** using `seaborn` for the best `K`.
7. **Visualized decision boundaries** using only 2 features (`PetalLengthCm`, `PetalWidthCm`).

---![image](https://github.com/user-attachments/assets/d73c0b41-6d49-4ee6-ac49-078e626cd746)
0         Iris-setosa
1         Iris-setosa
2         Iris-setosa
3         Iris-setosa
4         Iris-setosa
            ...      
145    Iris-virginica
146    Iris-virginica
147    Iris-virginica
148    Iris-virginica
149    Iris-virginica
Name: Species, Length: 150, dtype: object


## 📊 Results
- ✅ Best K: **3**
- ✅ Accuracy: **100%**
- ✅ Visualization: Clear and well-separated decision regions for all three species.

---K=1, Accuracy=0.98
K=2, Accuracy=0.98
K=3, Accuracy=1.00
K=4, Accuracy=0.98
K=5, Accuracy=1.00
K=6, Accuracy=1.00
K=7, Accuracy=1.00
K=8, Accuracy=1.00
K=9, Accuracy=1.00
K=10, Accuracy=1.00

## 📈 Visualization Samples

### Accuracy vs K
A line plot showing how the model’s accuracy changes with different values of `K`.
![image](https://github.com/user-attachments/assets/828d7948-25f9-4c5a-bc05-497d15144b73)


### Confusion Matrix
A heatmap to evaluate classification performance.
![image](https://github.com/user-attachments/assets/2bf2ee7b-6342-4328-a624-59b6e7a578c9)


### Decision Boundaries
A 2D plot showing how the KNN classifier differentiates between Iris species based on petal features.

---
![image](https://github.com/user-attachments/assets/7214987e-27fe-4a0f-a901-c7a6fcd8a729)


## 🚀 How to Run
1. Clone this repository or download the `Iris.csv` dataset.
2. Install required libraries:
   ```bash
   pip install pandas scikit-learn matplotlib seaborn
