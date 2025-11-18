# Scaling_ANN
# Improving Neural Network Performance Using Feature Scaling

This project demonstrates how **Standard Scaling** significantly improves the performance and training speed of a neural network model.

## 📂 Dataset
- The dataset used is available in the repository.
- A standard **train-test split** was applied before training.

---

## 🧠 Neural Network Architecture
A simple feed-forward neural network was used:

- **Input layer:** 1 feature  
- **Hidden layers:** 3 layers with **10 neurons** each (ReLU activation)  
- **Output layer:** 1 neuron (Sigmoid activation)  
- **Epochs:** 100  

---

## ❌ Model Training Without Scaling
Training the model directly on raw data produced poor results:

- **Accuracy:** ~0.68  
- **Loss:** did not improve (almost constant)  
- **Training time:** ~71 seconds  

The model struggled because unscaled input values slow down gradient descent and prevent proper convergence.

---

## ✔️ Model Training With Standard Scaling
After applying **StandardScaler** to the input features and training the same model:

- **Best Accuracy:** ~0.87  
- **Loss:** very low and consistently decreasing  
- **Training time:** ~70 seconds  

The model converged faster and performed significantly better.

---

## 📌 Conclusion
Scaling input data (especially using **Standard Scaling**) leads to:

- ✔️ Higher accuracy  
- ✔️ Faster convergence  
- ✔️ Lower loss  
- ✔️ More stable training  

Feature scaling ensures the neural network learns efficiently and avoids getting stuck due to large or inconsistent feature values.

---
