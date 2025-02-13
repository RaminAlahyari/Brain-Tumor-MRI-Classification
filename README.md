# Brain Tumor MRI Classification using Deep Learning

## 📌 Project Overview
This project focuses on **brain tumor classification** using **deep learning** techniques on MRI scans. The objective is to build a robust **Convolutional Neural Network (CNN)** to classify different types of brain tumors and improve model accuracy using **hyperparameter tuning, regularization, and transfer learning**.

## 🚀 Features & Methods Used
### 1️⃣ Data Preprocessing
- **ImageDataGenerator**: Used for data augmentation (rescaling, noise addition).
- **Data Splitting**: 80% training and 20% validation.
- **One-Hot Encoding** for multi-class classification.

### 2️⃣ Model Architecture & Training
- **CNN-based Model** with:
  - **Different filter sizes:** (3x3), (5x5)
  - **Activation functions:** ReLU & Tanh
  - **Pooling techniques:** MaxPooling
  - **Optimizers tested:** Adam, RMSprop, Adagrad, SGD
  - **Batch normalization** (explored but not implemented due to resource constraints)

### 3️⃣ Hyperparameter Tuning
- Grid search over parameters including:
  - **Filter sizes**: (3,3) & (5,5)
  - **Number of filters**: 32, 64
  - **Optimizers**: Adam, RMSprop, Adagrad, SGD
  - **Learning rates**: 0.001, 0.002, 0.01
  - **Dropout Rates**: 0.1 to 0.6 (Best at 0.4)
  
### 4️⃣ Fighting Overfitting
- **Reducing network capacity**
- **Adding dropout layers (0.4 rate worked best)**
- **L1-L2 Regularization**

### 5️⃣ Transfer Learning
- Explored architectures:
  - **VGG16**
  - **ResNet50**
  - **DenseNet** (Performed best)
- **Comparison with Baseline Model**:
  - DenseNet slightly underperformed compared to a simple CNN due to input resolution constraints.
  
## 🔥 Results & Performance
| Model      | Validation Accuracy | Test Accuracy |
|------------|--------------------|--------------|
| Base CNN  | 79.8% | 79.0% |
| Optimized CNN | 90.0% | 81.0% |
| DenseNet (Transfer Learning) | 79.0% | 74.0% |

## 📈 Future Enhancements
- Implement **hybrid architectures** (CNN + Attention mechanisms, Mask R-CNN)
- Train on **higher-resolution MRI images**
- Apply **advanced data augmentation techniques**

## 🏆 References
1. Pashaei et al. (2018) - CNN & Extreme Learning Machines for Brain Tumor Classification
2. Masood et al. (2022) - Mask RCNN with DenseNet-41 for MRI Analysis
3. Rasheed et al. (2024) - CNNs with Hybrid Attention Mechanisms for MRI Classification
4. Shorten & Khoshgoftaar (2019) - Survey on Image Data Augmentation in Deep Learning

## 📬 Contact
For queries, feel free to reach out via **GitHub Issues** or email!

_⭐ If you find this project useful, please give it a star! ⭐_
