1. DAAB: Dimensionality-Adaptive AutoML Benchmarking
Objective: Empirically compare AutoML frameworks across datasets of varying complexity.

Approach: Built a reproducible benchmarking pipeline evaluating 5 AutoML frameworks (Auto-sklearn, TPOT, AutoGluon, H2O, AutoKeras) across low-dimensional (Iris, 4 features) and high-dimensional (MNIST, 784 features) datasets. Applied statistical validation using Friedman-Nemenyi tests.

Key Innovations:

Adaptive budget allocation based on dataset complexity

Catastrophic failure registry for transparency

Checkpointing system for long-running experiments

Subprocess isolation to prevent crashes

Tech Stack: Python, scikit-learn, AutoML frameworks, Pandas, Matplotlib, Kaggle

Status: Under review for IEEE publication

2. Hyperparameter Optimization for Financial Fraud Detection
Objective: Evaluate HPO strategies on imbalanced financial classification tasks.

Approach: Benchmarked 6 classification algorithms (Logistic Regression, Naïve Bayes, kNN, Decision Tree, Random Forest, MLP) against 5 hyperparameter tuners (Random Search, Halving Search, Bayesian Optimization, Evolutionary Algorithm, Swarm Intelligence). Used Monte Carlo cross-validation (10 splits × 3-fold inner CV) on a real-world fraud dataset (~1M transactions, 3.5% fraud rate).

Key Insight: Some simpler tuning methods achieve competitive performance with significantly less computational cost.

Tech Stack: Python, scikit-learn, Optuna, sklearn-genetic-opt, PySwarm, OpenML
