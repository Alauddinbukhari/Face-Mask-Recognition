
# 🧑‍💻 Face-Mask-Recognition  
**Repository:** `Alauddinbukhari/Face-Mask-Recognition`  
**Visibility:** Public  

---

## 📌 Overview
**Face-Mask-Recognition** is a real-time face mask detection project built with **Python, Keras, and OpenCV**.  
It trains a **Convolutional Neural Network (CNN)** to classify images as **Mask** or **No Mask**, and integrates with a webcam feed to detect faces and display results live.  

---

## ⚙️ Features
- CNN model trained on custom dataset (`train/train` and `test/test`).  
- Real-time detection using Haar Cascade classifier.  
- Bounding boxes with labels:  
  - 🟥 **No Mask** → Red box  
  - 🟩 **Mask** → Green box  
- Data augmentation for robust training.  
- Model checkpointing (`model-010.h5`) and final saved model (`datamodel.h5`).  

---

## 🛠️ Tech Stack
- **Python 3.x**  
- **Keras / TensorFlow**  
- **OpenCV**  
- **NumPy**  
- **Scikit-learn**  

---

## 📂 Repository Structure
```
Face-Mask-Recognition/
├── train/                        # Training dataset
├── test/                         # Validation dataset
├── train.py                      # Model training script
├── recognize.py                  # Real-time detection script
├── model-010.h5                  # Saved trained model checkpoint
├── datamodel.h5                  # Final trained model
├── haarcascade_frontalface_default.xml # Haar Cascade for face detection
├── more about dataset.txt        # Dataset details
└── README.md                     # Project documentation
```

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/Alauddinbukhari/Face-Mask-Recognition.git
cd Face-Mask-Recognition
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Train the model
```bash
python train.py
```
This will train the CNN using images in `train/` and `test/` directories, and save the model as `datamodel.h5`.

### 4. Run real-time detection
```bash
python recognize.py
```
Press **ESC** to exit the webcam window.

---

## 📊 Model Architecture
- **Conv2D + MaxPooling** → Feature extraction  
- **Flatten** → Convert to 1D vector  
- **Dropout** → Prevent overfitting  
- **Dense layers** → Classification  
- **Softmax output** → Mask / No Mask  

---

## 👨‍🎓 Author
**Owner:** [Alauddinbukhari](https://github.com/Alauddinbukhari)  
- Full‑stack developer (Python, Java, React, Cloud)  
- Passionate about building scalable and secure applications  
- Open to freelance and contract opportunities  

