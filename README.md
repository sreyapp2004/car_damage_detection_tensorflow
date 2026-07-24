# 🚗 AI-Based Car Damage Detection System using Deep Learning

## 📌 Project Overview

The **AI-Based Car Damage Detection System** is a Computer Vision and Deep Learning project that automatically detects and classifies vehicle damage severity from car images.

The system uses a **Convolutional Neural Network (CNN)** model built with **TensorFlow and Keras** to classify vehicle damage into three categories:

* Minor Damage
* Moderate Damage
* Severe Damage

The model is trained on car damage images using image preprocessing and data augmentation techniques. It also supports **real-time damage prediction through a webcam using OpenCV**.

This project can help automate vehicle inspection processes and support applications such as insurance claim assessment and automotive maintenance.

---

# 🎯 Objectives

* Automate car damage severity classification using Artificial Intelligence.
* Reduce manual vehicle inspection effort.
* Apply Deep Learning techniques for image-based damage analysis.
* Provide real-time prediction using webcam input.
* Improve efficiency in vehicle damage assessment.

---

# 🛠️ Technologies Used

## Programming Language

* Python

## Deep Learning Frameworks

* TensorFlow
* Keras

## Computer Vision

* OpenCV

## Data Processing

* NumPy
* ImageDataGenerator

## Model Development

* CNN (Convolutional Neural Network)
* Batch Normalization
* Dropout Regularization
* Adam Optimizer

## Tools

* Jupyter Notebook
* VS Code
* Git & GitHub

---

# 🧠 Model Architecture

The project uses a custom CNN architecture consisting of:

```
Input Image (128x128x3)
          |
          ↓
Conv2D Layer (32 filters)
          |
Batch Normalization
          |
Max Pooling
          |
Conv2D Layer (64 filters)
          |
Batch Normalization
          |
Max Pooling
          |
Conv2D Layer (128 filters)
          |
Batch Normalization
          |
Max Pooling
          |
Flatten Layer
          |
Dense Layer (256 neurons)
          |
Dropout (0.5)
          |
Output Layer (3 classes)
          |
Minor / Moderate / Severe
```

---

# 📂 Dataset

The model is trained using a vehicle damage image dataset containing three damage categories:

```
Dataset
│
├── Minor Damage
│
├── Moderate Damage
│
└── Severe Damage
```

Dataset preprocessing includes:

* Image resizing to **128 × 128 pixels**
* Pixel normalization
* Data augmentation
* Training and validation split

---

# 🔄 Data Augmentation

To improve model generalization, the following augmentation techniques were applied:

* Rotation (30 degrees)
* Zoom transformation
* Horizontal flipping
* Brightness adjustment

Example:

```python
ImageDataGenerator(
    rescale=1./255,
    rotation_range=30,
    zoom_range=0.3,
    horizontal_flip=True,
    brightness_range=[0.7,1.3]
)
```

---

# ⚙️ Workflow

```
Car Image Input
        |
        ↓
Image Preprocessing
(Resize + Normalize)
        |
        ↓
CNN Feature Extraction
        |
        ↓
Deep Learning Classification
        |
        ↓
Damage Severity Prediction
        |
        ↓
Minor / Moderate / Severe
```

---

# ✨ Features

✅ Deep Learning based car damage classification
✅ Three-level damage severity prediction
✅ Image-based damage analysis
✅ Data augmentation for better accuracy
✅ Model saving and loading support
✅ Real-time webcam prediction using OpenCV
✅ Confidence score display for predictions

---

# 📊 Model Training

The model was trained using:

* Optimizer: Adam
* Learning Rate: 0.0001
* Loss Function: Categorical Cross Entropy
* Epochs: 10
* Batch Size: 32
* Input Size: 128 × 128

---

# 🚀 Installation & Setup

## 1. Clone the Repository

```bash
git clone https://github.com/yourusername/car-damage-detection.git
```

## 2. Navigate to Project Directory

```bash
cd car-damage-detection
```

## 3. Install Required Libraries

```bash
pip install -r requirements.txt
```

---

# 📦 Required Libraries

Create a `requirements.txt` file:

```
tensorflow
keras
opencv-python
numpy
split-folders
matplotlib
```

---

# ▶️ Running the Project

## Image Prediction

Run the Python file:

```bash
python main.py
```

The model will process the input image and display:

```
Prediction: Severe
Confidence: 95%
```

---

## Real-Time Webcam Detection

The system opens the webcam and predicts damage severity in real time.

Output example:

```
Car Damage Detection

Severe (92.45%)
```

Press:

```
q
```

to close the webcam window.

---

# 💾 Model Files

The trained model is saved as:

```
my_model.h5
```

Model architecture:

```
car_damage_detection.json
```

---

# 📁 Project Structure

```
Car-Damage-Detection/
│
├── dataset/
│
├── main.py
│
├── my_model.h5
│
├── model.json
│
├── requirements.txt
│
├── README.md
│
└── screenshots/
```

---

# 📸 Sample Output

(Add your screenshots here)

Example:

Input Image:

```
Car Image
```

Prediction:

```
Damage Type: Severe
Confidence: 95.2%
```

---

# 🔮 Future Enhancements

* Implement YOLO-based damage localization.
* Detect exact damaged regions in vehicles.
* Deploy as a web application using Flask/FastAPI.
* Add insurance cost estimation based on damage severity.
* Improve accuracy using transfer learning models such as ResNet or EfficientNet.

---

# 👩‍💻 Author

**Sreya P P**

Computer Science Graduate
AI & Machine Learning Enthusiast




