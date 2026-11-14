<div align="center">

# 🦁 K-Means Clustering — Interactive Masterclass & Visualizer
### **Lindenwood University — Interactive Data Science & Machine Learning Masterclass**

[![Live Interactive Lab](https://img.shields.io/badge/Launch_Interactive_Lab-Live_Demo-C5B358?style=for-the-badge&logo=googlechrome&logoColor=black)](https://sagarkalauni.github.io/k-mean-clustering/)
[![Course](https://img.shields.io/badge/Course-DSCI_35600-000000?style=for-the-badge&logo=academia&logoColor=C5B358)](#)
[![Author](https://img.shields.io/badge/Faculty-Sagar_Kalauni,_M.S.-1E293B?style=for-the-badge&logo=github&logoColor=white)](https://github.com/SagarKalauni)

</div>

---

## 📖 Overview

An interactive educational simulation of **K-Means Clustering (Lloyd's Algorithm)** built for Lindenwood University's Machine Learning curriculum. Students can dynamically place centroids, step through assignment and update iterations, inspect Voronoi decision regions, and analyze the Within-Cluster Sum of Squares (WCSS) Elbow curve in real time.

> 🔗 **Launch the Live Interactive Application:** [**https://sagarkalauni.github.io/k-mean-clustering/**](https://sagarkalauni.github.io/k-mean-clustering/)

---

### 📐 Mathematical Formulation

Given a dataset $\mathcal{X} = \{\mathbf{x}_1, \mathbf{x}_2, \dots, \mathbf{x}_n\} \subset \mathbb{R}^d$, K-Means partitions the observations into $K$ disjoint clusters $\mathcal{S} = \{S_1, S_2, \dots, S_K\}$ to minimize the **Within-Cluster Sum of Squares (WCSS / Inertia)**:

$$\underset{\mathcal{S}}{\arg\min} \sum_{k=1}^{K} \sum_{\mathbf{x}_i \in S_k} \left\| \mathbf{x}_i - \boldsymbol{\mu}_k \right\|_2^2$$

where $\boldsymbol{\mu}_k = \frac{1}{|S_k|} \sum_{\mathbf{x}_i \in S_k} \mathbf{x}_i$ is the centroid of cluster $S_k$.

1. **Assignment Step (Expectation):** Assign each observation to its nearest centroid under Euclidean metric:
   $$S_k^{(t)} = \left\{ \mathbf{x}_i : \left\| \mathbf{x}_i - \boldsymbol{\mu}_k^{(t)} \right\|_2^2 \le \left\| \mathbf{x}_i - \boldsymbol{\mu}_j^{(t)} \right\|_2^2 \ \forall j \in \{1, \dots, K\} \right\}$$
2. **Update Step (Maximization):** Recompute centroids as the sample mean of assigned points:
   $$\boldsymbol{\mu}_k^{(t+1)} = \frac{1}{\left|S_k^{(t)}\right|} \sum_{\mathbf{x}_i \in S_k^{(t)}} \mathbf{x}_i$$

---

## ✨ Key Interactive Features

- **Step-by-Step Lloyd's Algorithm:** Manually or automatically step through centroid initialization, point assignment, and centroid relocation.
- **Voronoi Partitioning Overlay:** Real-time geometric rendering of cluster boundaries in 2D feature space.
- **Interactive Elbow Method & Inertia Tracking:** Live plotting of Within-Cluster Sum of Squares (WCSS) across varying values of $K$ to identify optimal cluster cardinality.
- **Sensitivity to Initialization:** Demonstrate convergence to local optima and compare random initialization against K-Means++.

---

## 🎓 Pedagogical & Course Context

- **Institution:** Lindenwood University (*College of Science, Technology, and Health*)
- **Course Curriculum:** DSCI 35600 — Machine Learning
- **Instructor & Author:** **Sagar Kalauni, M.S.** (*Full-Time Faculty in Data Science*)
- **Tech Stack:** HTML5, Tailwind CSS, **D3.js** (Dynamic Data Visualization), **MathJax** (LaTeX Mathematical Rendering), Vanilla ES6+ JavaScript (Zero-Dependency Client-Side Execution).

---

## 🚀 Running Locally

Because this visualizer is engineered as a self-contained, zero-build client-side application, you can run it immediately in any modern browser:

```bash
# Clone the repository
git clone https://github.com/SagarKalauni/k-mean-clustering.git

# Navigate into the project directory
cd k-mean-clustering

# Open index.html directly in your browser or serve locally:
python -m http.server 8000
```

---

## 🔗 Explore the Complete Interactive Masterclass Suite

| Module | Topic | Live Link |
| :--- | :--- | :---: |
| **Linear Regression** | Ordinary Least Squares & Residual Minimization | [Launch](https://sagarkalauni.github.io/linear-regression/) |
| **Logistic Regression** | Sigmoid Probabilities & Binary Cross-Entropy | [Launch](https://sagarkalauni.github.io/logistic-regression/) |
| **Regularization ($L_1 / L_2$)** | Lasso vs. Ridge Constraint Geometry | [Launch](https://sagarkalauni.github.io/Regularization/) |
| **K-Nearest Neighbors** | Instance-Based Learning & Distance Metrics | [Launch](https://sagarkalauni.github.io/knn/) |
| **Support Vector Machine** | Maximum-Margin Hyperplanes & Soft Margin $C$ | [Launch](https://sagarkalauni.github.io/support-vector-machine/) |
| **RBF Kernel SVM** | Non-Linear Kernel Trick & $(\gamma, C)$ Tuning | [Launch](https://sagarkalauni.github.io/rbf-kernel-svm/) |
| **Decision Tree (CART)** | Recursive Splitting, Gini & Entropy | [Launch](https://sagarkalauni.github.io/decision-tree/) |
| **Random Forest** | Bagging & Ensemble Variance Reduction | [Launch](https://sagarkalauni.github.io/random-forest/) |
| **Voting Classifier** | Hard Majority vs. Soft Probability Voting | [Launch](https://sagarkalauni.github.io/voting-classifier/) |
| **K-Means Clustering** | Lloyd's Algorithm, Voronoi & Elbow WCSS | [Launch](https://sagarkalauni.github.io/k-mean-clustering/) |
| **Confusion Matrix** | Precision, Recall, Specificity & $F_1$-Score | [Launch](https://sagarkalauni.github.io/confusion-matrix/) |
| **Confidence vs. Prediction Intervals** | Mean Response vs. Individual Uncertainty | [Launch](https://sagarkalauni.github.io/confidence-and-prediction-interval/) |
| **Bootstrapping** | Non-Parametric Resampling with Replacement | [Launch](https://sagarkalauni.github.io/bootstrap/) |
| **Q-Q Plot** | Gaussian Normality & Tail Diagnostics | [Launch](https://sagarkalauni.github.io/qq-plot/) |
| **Train-Test Split & CV** | Holdout Partitioning & $K$-Fold Cross-Validation | [Launch](https://sagarkalauni.github.io/split/) |
| **One-Hot Encoding** | Categorical Expansion & Dummy Variable Trap | [Launch](https://sagarkalauni.github.io/one-hot-encoding/) |

---

<div align="center">
  <sub>Developed with ❤️ for Data Science students by <a href="https://github.com/SagarKalauni">Sagar Kalauni</a> · <a href="https://sagarkalauni.github.io">Portfolio</a></sub>
</div>
