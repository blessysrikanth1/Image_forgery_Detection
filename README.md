# 🖼️ Image Forgery Detection Using ELA and CNN

## 📌 Project Overview  
Image forgery has become a significant concern due to the availability of advanced editing tools. This project aims to **detect forged images** using **Error Level Analysis (ELA)** and **Convolutional Neural Networks (CNNs)**.  
- **ELA** highlights tampered regions in an image by analyzing compression errors.  
- **CNN** is trained to classify real vs. fake images based on ELA-processed inputs.  

## 🌟 Key Features  
✅ Detects manipulated or forged images  
✅ Uses **Error Level Analysis (ELA)** for preprocessing  
✅ Deep learning-based **CNN model** for classification  
✅ Works with **JPEG and PNG** image formats  
✅ Generates a **heatmap** for visualization of forged areas  

---

## 🔬 How It Works  
This project follows a **two-step approach**:  

### **1️⃣ Preprocessing with Error Level Analysis (ELA)**  
ELA works by compressing an image and comparing it with the original to detect inconsistencies.  
- If an image is **unaltered**, all regions degrade similarly.  
- If an image is **forged**, manipulated areas degrade differently due to inconsistent compression.  

**Example:**  
Original Image → Compressed → Difference Computed → Output ELA Image  

### **2️⃣ Classification Using CNN**  
A **Convolutional Neural Network (CNN)** is trained to classify real vs. fake images using ELA images as input.  
- The model learns pixel-level anomalies that indicate forgery.  
- The CNN is fine-tuned for high accuracy.  

---

## 🛠️ Technologies Used  
🔹 **Python** - Core programming language  
🔹 **OpenCV** - Image processing  
🔹 **TensorFlow/Keras** - Deep learning framework  
🔹 **Matplotlib** - Visualization  
🔹 **NumPy & Pandas** - Data manipulation  

---

## 📂 Dataset Used  
The dataset contains:  
- **Real images** (original, unmodified)  
- **Fake images** (edited using Photoshop/GANs)  
- **Generated ELA images** for training  
