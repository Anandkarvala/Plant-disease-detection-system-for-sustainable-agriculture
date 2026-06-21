# 🌿 Plant Leaf Disease Detection Using Convolutional Neural Networks (CNN)

## 📌 Project Overview

This project focuses on detecting and classifying plant leaf diseases using a Deep Learning-based Convolutional Neural Network (CNN). The model is trained on the PlantVillage dataset containing images of healthy and diseased plant leaves across multiple crop species.

The system automatically identifies plant diseases from leaf images, helping farmers and agricultural experts take timely action to improve crop health and productivity.

---

## 🎯 Objectives

* Detect plant diseases from leaf images.
* Classify images into 38 disease categories.
* Improve agricultural productivity through early disease identification.
* Build an accurate and scalable deep learning model for disease diagnosis.

---

## 📂 Dataset

**Dataset:** PlantVillage Dataset

The dataset contains **over 80,000 images** of healthy and diseased plant leaves belonging to multiple crops such as:

* Apple
* Blueberry
* Cherry
* Corn
* Grape
* Orange
* Peach
* Pepper
* Potato
* Raspberry
* Soybean
* Squash
* Strawberry
* Tomato

### Number of Classes

* 38 Plant Disease Classes

Examples include:

* Apple Scab
* Black Rot
* Cedar Apple Rust
* Early Blight
* Late Blight
* Leaf Mold
* Bacterial Spot
* Healthy Leaves

---

## 🛠 Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Pandas
* OpenCV
* Matplotlib
* Seaborn
* Google Colab

---

## 🏗 Model Architecture

The CNN architecture consists of:

1. Conv2D Layer (32 Filters, 7×7 Kernel)
2. MaxPooling Layer
3. Conv2D Layer (64 Filters, 5×5 Kernel)
4. MaxPooling Layer
5. Conv2D Layer (128 Filters, 3×3 Kernel)
6. Conv2D Layer (256 Filters, 3×3 Kernel)
7. MaxPooling Layer
8. Flatten Layer
9. Dense Layer (128 Neurons)
10. Dense Layer (64 Neurons)
11. Output Layer (38 Classes, Softmax Activation)

### Model Parameters

* Total Parameters: 26,125,990
* Trainable Parameters: 26,125,990

---

## 🔄 Data Preprocessing

The following preprocessing techniques were applied:

* Image Rescaling (1/255)
* Image Resizing (224 × 224)
* Data Augmentation

  * Rotation
* Train-Validation Split
* Batch Processing

---

## ⚙ Training Configuration

| Parameter     | Value                       |
| ------------- | --------------------------- |
| Image Size    | 224 × 224                   |
| Batch Size    | 164                         |
| Optimizer     | Adam                        |
| Loss Function | Categorical Crossentropy    |
| Epochs        | 5                           |
| Metrics       | Accuracy, Precision, Recall |

### Callbacks Used

* EarlyStopping
* ModelCheckpoint
* ReduceLROnPlateau

---

## 📈 Model Performance

### Validation Results

| Metric               | Score  |
| -------------------- | ------ |
| Validation Accuracy  | 89.84% |
| Validation Precision | 91.43% |
| Validation Recall    | 88.17% |
| Validation Loss      | 0.3244 |

### Test Results

| Metric    | Score  |
| --------- | ------ |
| Accuracy  | 90.50% |
| Precision | 92.30% |
| Recall    | 88.97% |
| Loss      | 0.2850 |

---

## 📊 Results

The CNN model achieved over **90% test accuracy** in classifying plant diseases across 38 categories, demonstrating strong performance for automated plant disease diagnosis.

---

## 💾 Saved Model

The trained model is saved as:

```bash
PDDS.keras
```

This model can be loaded later for prediction and deployment purposes.

---

## 🚀 How to Run the Project

### Clone Repository

```bash
git clone https://github.com/Anandkarvala/plant-leaf-disease-detection.git
```

### Navigate to Project Folder

```bash
cd plant-leaf-disease-detection
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Jupyter Notebook

```bash
jupyter notebook
```

Open:

```bash
plant_leaf_disease_detection.ipynb
```

Run all cells to train and evaluate the model.

---

## 🌱 Future Enhancements

* Real-time disease detection using a mobile camera.
* Web application deployment using Flask.
* Explainable AI (XAI) integration.
* Transfer Learning using ResNet50, EfficientNet, and MobileNet.
* Disease treatment recommendation system.

---

## 👨‍💻 Author

**Karvala Anand**

B.Tech – Computer Science and Engineering

GitHub: https://github.com/Anandkarvala

---

## 📜 License

This project is developed for educational, research, and academic purposes.
