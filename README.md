SVM Classification on Breast Cancer Dataset

This project demonstrates how to apply Support Vector Machines (SVM) for binary classification using both Linear and RBF kernels. It includes preprocessing, model training, hyperparameter tuning, visualization, and evaluation.

🚀 Project Overview

The goal is to:

Build an SVM classifier for a binary cancer diagnosis prediction task

Compare Linear SVM vs RBF SVM

Apply feature scaling, cross-validation, and hyperparameter tuning

Visualize decision boundaries in 2D using PCA

Evaluate the best model with detailed metrics

Dataset used (uploaded locally):

/mnt/data/breast-cancer.csv

🧠 What You Will Learn

Understanding how margins affect classification

Using the kernel trick for non-linear decision boundaries

Tuning SVM hyperparameters like C and gamma

Evaluating models using accuracy, confusion matrix, and classification report

Visualizing SVM decision boundaries in reduced dimensions

🛠 Technologies Used

Python

NumPy

Pandas

Scikit-learn

Matplotlib

PCA (for visualization)

📂 Project Structure
│── breast-cancer.csv          # Dataset
│── svm_classification.py      # Full SVM code
│── README.md                  # Project documentation

📥 How to Run

Install dependencies:

pip install numpy pandas scikit-learn matplotlib


Run the project:

python svm_classification.py


Make sure the dataset path matches:

df = pd.read_csv("/mnt/data/breast-cancer.csv")

📊 Key Results

The project prints:

Accuracy for Linear SVM

Accuracy for RBF SVM

Best parameters from GridSearchCV

Best model performance on test data

Confusion Matrix

Classification Report

PCA-based decision boundary plot

📈 Decision Boundary Visualization

Since real datasets are high-dimensional, PCA (2D) is used to visualize the classifier’s separation capability.

🧪 Evaluation Metrics

The project includes:

Accuracy Score

Confusion Matrix

Precision, Recall, F1-score

These help measure real-world performance on medical diagnosis tasks.

⚙️ Hyperparameter Tuning

GridSearchCV is used with:

C: [0.1, 1, 10, 100]
gamma: ["scale", 0.01, 0.001]
kernel: ["rbf"]


This ensures the best combination of margin width and kernel influence.

📝 Future Improvements

Try more kernels (poly, sigmoid)

Use class balancing techniques

Integrate pipeline & automated scaling

Deploy the model (Flask/FastAPI + UI)

👨‍💻 Author

SSV SAI DURGA PRASAD ADAPAKA
