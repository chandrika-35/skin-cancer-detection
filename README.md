# 🩺 Skin Cancer Detection Using Deep Learning

## 📌 Overview

**Skin Cancer Detection Using Deep Learning** is a web-based application that leverages **EfficientNetB0 Transfer Learning** to classify dermoscopic skin lesion images as **Benign** or **Malignant**. The project combines **Computer Vision**, **Deep Learning**, and **Explainable AI (Grad-CAM)** to assist in the early detection of skin cancer.

Users can upload a skin lesion image through a simple Flask web interface and receive:

* Skin lesion classification
* Confidence score
* Malignancy probability
* Risk level assessment
* Grad-CAM heatmap for model interpretability

> **Note:** This application is intended for educational and research purposes and should not be used as a substitute for professional medical diagnosis.

---

# 🚀 Features

* Upload skin lesion images (JPG, JPEG, PNG)
* Automatic image preprocessing
* Hair artifact removal
* Image resizing and normalization
* Data augmentation during training
* Binary classification (Benign / Malignant)
* Confidence score prediction
* Malignancy probability estimation
* Risk level assessment
* Grad-CAM explainability visualization
* Responsive Flask web interface with Bootstrap 5

---

# 🛠️ Technologies Used

## Frontend

* Flask
* HTML5
* CSS3
* Bootstrap 5
* JavaScript

## Backend

* Python

## Deep Learning & Computer Vision

* TensorFlow
* Keras
* OpenCV
* NumPy
* Pandas
* Matplotlib
* Scikit-Learn

---

# 🤖 Deep Learning Models

The project supports transfer learning using modern CNN architectures such as:

* EfficientNetB0 *(Primary Model)*
* ResNet50
* MobileNetV2

Current implementation uses **EfficientNetB0** for binary skin lesion classification.

---

# 📂 Dataset

**Dataset:** HAM10000 (Human Against Machine with 10,000 Training Images)

### Dataset Includes

* Dermoscopic skin lesion images
* Lesion categories
* Benign/Malignant labels

---

# 📁 Project Structure

```text
Skin-Cancer-Detection/
│
├── app.py                    # Flask application
├── train.py                  # Model training
├── predict.py                # Prediction script
├── gradcam.py                # Grad-CAM visualization
├── prepare_dataset.py        # Dataset preprocessing
├── config.py                 # Configuration settings
├── utils.py                  # Utility functions
├── requirements.txt
├── README.md
│
├── dataset/
│   ├── train/
│   ├── validation/
│   └── test/
│
├── models/
│   └── efficientnet_model.h5
│
├── static/
│   ├── uploads/
│   ├── gradcam/
│   └── css/
│
└── templates/
    ├── index.html
    └── result.html
```

---

# ⚙️ System Modules

## 1. Image Upload

Users upload dermoscopic skin lesion images through the web interface.

## 2. Image Preprocessing

The uploaded image undergoes several preprocessing steps:

* Resize to **224 × 224**
* Pixel normalization
* Hair artifact removal
* Image enhancement

During training:

* Data augmentation
* Rotation
* Flipping
* Zooming

## 3. Model Prediction

The preprocessed image is passed through the trained **EfficientNetB0** model to generate predictions.

## 4. Result Display

The application displays:

* Predicted Class
* Confidence Score
* Malignancy Probability
* Risk Level

## 5. Explainability (Grad-CAM)

A Grad-CAM heatmap is generated to highlight image regions that influenced the model's prediction, improving transparency and interpretability.

---

# 🔄 Workflow

```text
Upload Image
      │
      ▼
Image Preprocessing
      │
      ▼
EfficientNetB0 Prediction
      │
      ▼
Confidence & Risk Assessment
      │
      ▼
Grad-CAM Heatmap Generation
      │
      ▼
Display Results
```

---

# 📊 Model Evaluation

The model is evaluated using standard classification metrics:

* Accuracy
* Precision
* Recall
* F1-Score
* AUC-ROC

---

# ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Skin-Cancer-Detection.git
```

Move into the project directory:

```bash
cd Skin-Cancer-Detection
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# 📦 Prepare Dataset

```bash
python prepare_dataset.py
```

---

# 🏋️ Train the Model

```bash
python train.py
```

The trained model will be saved in the **models/** directory.

---

# ▶️ Run the Application

```bash
python app.py
```

Open your browser and visit:

```text
http://127.0.0.1:5000
```

---

# 🎯 Expected Outcomes

* Accurate skin lesion classification
* Real-time prediction results
* Explainable AI-assisted decision making
* Improved support for early skin cancer detection
* User-friendly and responsive web interface

---

# 🔮 Future Enhancements

* Multi-class skin lesion classification
* Clinical decision support features
* Cloud deployment (AWS/Azure/GCP)
* Mobile application integration
* User authentication
* Database integration
* Patient history management
* Advanced Explainable AI techniques
* Model optimization for edge devices

---

# 📖 Conclusion

This project demonstrates the application of **Deep Learning**, **Transfer Learning**, and **Computer Vision** in healthcare. By combining an EfficientNetB0-based skin lesion classifier with **Grad-CAM Explainable AI**, the system provides an accessible and interpretable tool for assisting in the early detection of skin cancer.

Although intended primarily for educational and research purposes, the project showcases how AI can support healthcare professionals by providing accurate predictions along with visual explanations that enhance model transparency.

---

# 👨‍💻 Author

N.chandrika

---

# 📄 License

This project is intended for educational and research purposes. Please ensure compliance with the HAM10000 dataset license and applicable healthcare regulations before using or distributing the project.

