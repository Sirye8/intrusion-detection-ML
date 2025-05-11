# Network Anomaly Detection  
**A machine learning pipeline to detect cybersecurity intrusions in simulated network traffic using statistical analysis (z-score) and probabilistic classifiers (Naive Bayes).**

---

## Project Overview  
This project aims to identify anomalous network connections in a simulated US Air Force LAN environment. It follows a three-stage approach:  
1. **Exploratory Data Analysis**: Statistical summaries, PDF/PMF/CDF visualization, and correlation analysis.  
2. **Z-Score Thresholding**: Detect outliers using dynamic z-score thresholds and evaluate performance metrics.  
3. **Naive Bayes Classification**: Implement a custom Naive Bayes estimator and compare it with Scikit-learn models (Gaussian, Multinomial, Bernoulli).  

**Key Features**:  
- Focus on **high recall** to minimize undetected threats in cybersecurity contexts.  
- Custom distribution fitting (24+ probability distributions) for numerical features.  
- Conditional PMF analysis for categorical features.  
- Performance benchmarking across multiple thresholds and algorithms.

---

## Repository Structure  
- **Milestone 1.py**: Data discovery, PMF/CDF, and correlation analysis  
- **Milestone 2.py**: Z-score anomaly detection and PDF fitting  
- **Milestone 3.py**: Naive Bayes classifier implementation  
- **Train_data.csv**: Dataset (simulated US Air Force LAN traffic) 

---

## Dependencies  
**Core Libraries**:  
```python
pandas >= 2.0.0        # Data manipulation and analysis  
numpy >= 1.24.0        # Numerical computations  
matplotlib >= 3.7.0    # Visualization (PDF/PMF/CDF plots)  
scipy >= 1.10.0        # Statistical distributions and fitting  
scikit-learn >= 1.3.0  # Naive Bayes classifiers (Gaussian/Multinomial/Bernoulli)
```

---

## Results
- **Best-performing model**: Bernoulli Naive Bayes (Accuracy: `0.95` Precision: `0.91` Recall: `0.93`).
- **Focus**: High recall to minimize undetected threats.
- Recall-driven design ensures 93%+ detection rate for anomalies, critical for security applications.
