Skin Cancer Detection Using Deep Learning

📌 Project Overview

Skin Cancer Detection is a Deep Learning-based web application that classifies skin lesions as Benign or Malignant using dermoscopic images. The system assists in the early detection of skin cancer by leveraging Convolutional Neural Networks (CNNs) and Explainable AI techniques.

Users can upload a skin lesion image and receive a prediction along with confidence scores and a Grad-CAM heatmap for model interpretability.

---

🚀 Features

- Upload skin lesion images (JPEG/PNG)
- Image preprocessing and enhancement
- Benign/Malignant classification
- Malignancy probability prediction
- Risk level assessment
- Grad-CAM heatmap visualization
- User-friendly Flask web interface

---

🛠️ Technologies Used

Frontend

- Flask

Machine Learning & Deep Learning

- TensorFlow
- Keras
- OpenCV
- NumPy
- Matplotlib

Models

- EfficientNetB0
- ResNet50
- MobileNetV2

---

📂 Dataset

Dataset: HAM10000 (Human Against Machine with 10000 Training Images)

Dataset Features

- Skin Lesion Images
- Lesion Type
- Benign/Malignant Labels

---

⚙️ System Modules

1. Image Upload

Accepts dermoscopic images through the Flask interface.

2. Image Preprocessing

- Resize images to 224×224
- Normalize pixel values
- Data augmentation
- Hair artifact removal

3. Model Prediction

Generates predictions using a fine-tuned CNN model.

4. Result Display

Shows:

- Classification Result
- Confidence Score
- Risk Level

5. Explainability Report

Generates a Grad-CAM heatmap highlighting important regions in the image.

---

🔄 Workflow

1. Upload Image
2. Preprocess Image
3. Run CNN Model
4. Generate Prediction
5. Display Results
6. Generate Grad-CAM Visualization

---

📊 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- AUC-ROC

---

▶️ How to Run

Install Dependencies

pip install -r requirements.txt

Run Application

python app.py

Open Browser

http://127.0.0.1:5000

---

🎯 Expected Outcome

- Accurate skin lesion classification
- Real-time prediction results
- Improved diagnostic support
- Explainable AI-based decision making
- Easy-to-use web interface

---

🔮 Future Enhancements

- Multi-class lesion classification
- Mobile application integration
- Cloud deployment
- Clinical decision support features
- Advanced explainability methods

---

📖 Conclusion

This project demonstrates the application of Deep Learning and Computer Vision in healthcare. By combining accurate skin lesion classification with explainable AI, the system provides a practical solution for assisting in the early detection of skin cancer while offering a seamless user experience# skin-cancer-detection
