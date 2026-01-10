# Brain-Tumor-Optimization-CNN

# Optimization Dynamics in CNN-Based Brain Tumor Detection
**A Comparative Study of SGD, Adam, RMSprop, and AdamW**

##  Project Overview
This project benchmarks four major optimization algorithms to determine the most effective method for identifying brain tumors in MRI scans. Using a custom 4-block CNN architecture, this study analyzes convergence speed, stability (σ), and generalization ability.

### 🚀 Key Performance Results
| Optimizer | Accuracy | AUC Score | Best Feature |
| :--- | :--- | :--- | :--- |
| **AdamW** | **98.48%** | 0.9966 | Highest overall precision |
| **SGD** | 97.61% | **0.9980** | Best generalization (Lowest Gap) |
| **Adam** | 97.94% | 0.9966 | Most stable (Lowest σ: 0.0033) |


<img width="686" height="625" alt="PERFORMANCE" src="https://github.com/user-attachments/assets/a0f89d95-70a2-44da-9b26-51d33acf537f" />

###Validation Accuracy   Loss per Epoch:
<img width="1473" height="873" alt="Validation Accuracy   Loss per Epoch" src="https://github.com/user-attachments/assets/b47db6bc-da11-4c61-aa8d-336ca624e02b" />



---

##  Methodology (STAR)
- **Situation:** Manual MRI analysis is error-prone. Automated systems need an "optimal" optimizer to ensure clinical reliability.
- **Task:** Compare 4 optimizers under identical conditions (60 epochs, 3e-4 learning rate) using 4,600 Kaggle MRI images.
- **Action:** Developed a **PyTorch-based CNN** with 4 convolutional blocks. Implemented `ReduceLROnPlateau` and conducted a parametric study on optimization dynamics.
- **Result:** written a research paper identifying AdamW as the best for accuracy and SGD as the best for avoiding overfitting.

---
