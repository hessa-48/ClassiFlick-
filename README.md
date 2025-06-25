# 🧠 ClassiFlick — Image Classification with CNN

A deep learning project that explores multiple CNN architectures to classify images from the CIFAR-10 dataset. The project includes both custom-built CNN models and transfer learning using VGG16 and ResNet50, with deployment as a web app.

---

## 👥 Team Members
- **Hassa Mohammed**
- **Amjad Aloufi**
- **Arwa AbuFeeh**

---

## 📦 Dataset
**CIFAR-10**  
- 60,000 color images (32×32 pixels)  
- 10 balanced classes:
  `airplane`, `automobile`, `bird`, `cat`, `deer`, `dog`, `frog`, `horse`, `ship`, `truck`

---

## ⚙️ Model Architectures

### 🔧 Custom CNN Models

#### Model 1
- Basic architecture with normalization, ReLU activation, and dropout
- Optimizer: Adam | Epochs: 20
- **Accuracy**: 73.1%

#### Model 2
- Added data augmentation (rotation, flip, zoom)
- Deeper filters (64–128–256), batch normalization, dropout
- Early stopping and learning rate reduction
- **Accuracy**: 81.2%

#### Model 3
- Advanced augmentation + 4 convolutional blocks + 50% dropout
- Dense layer with 512 neurons
- **Accuracy**: 90.17%

---

### 🧠 Transfer Learning Models

#### ResNet50
- 50-layer deep residual network
- Optimizer: SGD
- **Train Accuracy**: 91%  
- **Validation Accuracy**: 88%  
- Observed overfitting

#### ✅ VGG16 (Best Model)
- Stacked convolutional layers
- Optimizer: SGD
- **Train Accuracy**: 96%  
- **Validation Accuracy**: 93%  
- Best generalization and ease of deployment

---

## 📊 Results Summary

| Model     | Accuracy   |
|-----------|------------|
| Model 1   | 73.1%      |
| Model 2   | 81.2%      |
| Model 3   | 90.17%     |
| ResNet50  | 92%        |
| **VGG16** | **95%**    |

> VGG16 showed the best balance between performance and generalization.

---

## 🔑 Key Insights
- Data augmentation significantly boosts generalization
- Transfer learning outperforms custom CNNs in accuracy and training time
- Dropout and batch normalization help reduce overfitting
- VGG16 proved to be the most practical and effective model

---

## 🚀 Deployment

The best model (VGG16) was deployed as a web app using **Flask**:

- Saved as `cifar10_best_model.h5`
- Flask backend API for image upload and prediction
- Frontend built with HTML/CSS for user interaction
- Visualized:
  - Real-time predictions
  - Accuracy/loss over time

---

## 🛠 Tech Stack
- Python  
- TensorFlow / Keras  
- Flask (backend)  
- HTML/CSS (frontend)  
- VGG16, ResNet50  
- CIFAR-10 Dataset

---

## 📬 Contact
For questions or collaboration opportunities, feel free to reach out!

