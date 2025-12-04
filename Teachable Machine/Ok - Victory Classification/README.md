# **✌️ Ok - Victory Hand Gesture Classification 👌**

> *"In the world of silent communication, your hands speak volumes!"*

---

## **🚀 1. Methodology**

Welcome to the fascinating world of **hand gesture recognition**! This project harnesses the power of Google's Teachable Machine platform to create an intelligent image classification model that can distinguish between two iconic hand gestures:

### 🎯 **Target Gestures:**
- **👌 Ok gesture**: The classic "OK" sign - a universal symbol of approval and perfection
- **✌️ Victory gesture**: The legendary "V" sign - representing victory, peace, and triumph

<!-- Add methodology diagram/flowchart here -->
![Methodology Diagram](placeholder-for-methodology-image.png)

The model leverages **TensorFlow.js** architecture, bringing machine learning directly to your browser for seamless, real-time hand gesture recognition experiences.

---

## **🧠 2. Description**

Step into the future of **human-computer interaction**! The Ok - Victory Classification model is a cutting-edge, lightweight machine learning solution that transforms the way we communicate with technology through natural hand gestures.

<!-- Add project banner/hero image here -->
![Project Banner](placeholder-for-project-banner.png)

**Key Features:**
- Real-time gesture recognition
- Browser-based implementation using TensorFlow.js
- Lightweight model suitable for edge deployment
- Pre-trained on custom dataset of hand gestures
- High accuracy classification between Ok and Victory gestures

**Technical Specifications:**
- Model Framework: TensorFlow.js v1.7.4
- Teachable Machine Version: 2.4.10
- Input Image Size: 224x224 pixels
- Number of Classes: 2 (Ok, Victory)
- Model Format: TensorFlow.js web format

## **3. Input / Output**
**Input:**
- Image: 224x224 pixel RGB images containing hand gestures
- Format: JPEG, PNG, or real-time webcam feed
- Requirements: Clear visibility of hand gesture against contrasting background

**Output:**
- Classification result with confidence scores
- Predicted class: "Ok" or "Victory"
- Confidence percentage for each gesture class

## **4. Model Files**
This project contains the following files:
- `model.json`: TensorFlow.js model architecture and configuration
- `weights.bin`: Pre-trained model weights
- `metadata.json`: Model metadata including labels and specifications

## **5. Usage Instructions**

### **Loading the Model:**
```javascript
// Load the model
const modelURL = './model.json';
const model = await tf.loadLayersModel(modelURL);
```

### **Making Predictions:**
```javascript
// Preprocess image and make prediction
const prediction = await model.predict(preprocessedImage);
const result = prediction.dataSync();
```

### **Integration Example:**
```html
<script src="https://cdn.jsdelivr.net/npm/@tensorflow/tfjs"></script>
<script>
    async function classifyGesture(imageElement) {
        const model = await tf.loadLayersModel('./model.json');
        // Add your preprocessing and prediction logic here
    }
</script>
```

## **6. Training Information**
- **Training Date:** December 4, 2025
- **Dataset:** Custom hand gesture images
- **Ok Samples:** 30 images
- **Victory Samples:** 20 images
- **Total Training Images:** 50 images

## **7. Performance**
The model has been optimized for:
- Fast inference on web browsers
- Real-time gesture recognition
- Minimal computational requirements
- Cross-platform compatibility

## **8. License**
This project uses Google's Teachable Machine platform and follows their terms of service for model creation and deployment.