# 🚀 CUDA-PSO Optimized Intrusion Detection System (IDS)

## 📌 Overview
This project implements an advanced Intrusion Detection System (IDS) using a Neural Network optimized with Particle Swarm Optimization (PSO) and accelerated using CUDA (GPU computing).

The model is trained on the NSL-KDD dataset to classify network traffic as either normal or attack.

---

## 🎯 Features
- Neural Network using PyTorch
- Hyperparameter tuning using PSO
- GPU acceleration with CUDA
- Performance comparison (before vs after optimization)
- Visualization of results (graphs, confusion matrix, speedup)

---

## 🗂 Dataset
- NSL-KDD Dataset
  - KDDTrain+.txt
  - KDDTest+.txt

---

## ⚙️ Technologies Used
- Python
- PyTorch
- NumPy, Pandas
- Scikit-learn
- PySwarms
- Matplotlib, Seaborn
- CUDA (GPU)

---

## 🧪 Methodology

### 1. Data Preprocessing
- Label encoding for categorical features
- Feature scaling using StandardScaler
- Converted labels to binary:
  - normal → 0
  - attack → 1

---

### 2. Model Architecture
- Input Layer (41 features)
- Hidden Layer (64 neurons, ReLU)
- Dropout Layer (optimized)
- Output Layer (Sigmoid)

---

### 3. PSO Optimization
- Optimized parameters:
  - Learning Rate
  - Dropout Rate
- Objective: Minimize loss

---

### 4. Training
- Base Model (default parameters)
- Optimized Model (PSO-tuned parameters)

---

## 📊 Results

| Metric     | Base Model | Optimized Model |
|------------|-----------|----------------|
| Accuracy   | 94.5%     | 98%+           |
| Precision  | 93%       | 97%+           |
| Recall     | 91%       | 98%+           |
| F1 Score   | 92%       | 98%+           |

---

## ⚡ Performance

- CPU Execution Time: 52.4 minutes  
- GPU Execution Time: 4.5 minutes  
- Speedup: ~11× faster  

---

## 📈 Outputs
- PSO convergence graph
- Confusion matrix
- Performance comparison charts
- Execution time comparison
- Speedup visualization

---

## ▶️ How to Run

### 1. Clone Repository
```bash

https://github.com/EerthineniAnupama/intrusion_detection_system_scl
```


### 2. Install Dependencies

```bash

pip install torch pandas numpy scikit-learn matplotlib seaborn pyswarms cupy-cuda12x numba
```

### 3. Run the Project
```
python code.py
```


📁 Project Structure
```



├── code.py / code.ipynb
├── KDDTrain+.txt
├── KDDTest+.txt
├── code.py
└── README.md
```

🧠 Conclusion

The CUDA-PSO optimized model significantly improves both performance and computation speed compared to the baseline neural network.



