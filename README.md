# Integrated-Fall-Detection-and-Action-Recognition-System-with-Real-Time-Alert-Notification

A robust real-time system for Human Activity Recognition (HAR) and Fall Detection using deep learning with attention mechanisms. This solution enhances safety in healthcare, elder care, and surveillance by classifying activities and triggering automated alerts upon detecting fall events.

## 🚀 Key Features

- 🎥 **Real-Time Video Processing**  
  Processes video frames in real-time to recognize human activities and falls.

- 🧩 **Attention-Enhanced Deep Learning Models**  
  Uses spatial and channel attention mechanisms (SE blocks) to improve feature focus and classification accuracy.

- 🔍 **Activity Recognition**  
  Detects complex ADLs like walking, hopping, picking objects, sitting, and kneeling.

- ⚠️ **Fall Detection with Alerts**  
  Identifies multiple fall types (forward, backward, left, right, from sitting) and sends SMS alerts via Twilio API.

- 📈 **High Accuracy**  
  - Fall Detection Accuracy: 99.77%  
  - Action Recognition Accuracy: 98.80%

- 🧪 **Data Augmentation**  
  Includes rotation, zoom, flip, brightness/contrast adjustments, and cropping for better generalization.

- 🛠️ **Model Ensemble**  
  Combines predictions using soft probabilities and majority voting for robust classification.

- 📲 **SMS Notification System**  
  Integrates Twilio API for real-time caregiver alerts on fall detection.

## 📊 Performance Summary

| Task              | Model                      | Accuracy | F1 Score | Special Mechanism             |
|-------------------|----------------------------|----------|----------|-------------------------------|
| Fall Detection    | Attention CNN              | 99.77%   | 1.00     | Spatial & Channel Attention   |
| Activity Recognition | Alternate Attention CNN | 98.80%   | 0.99     | Layer-wise Enhanced Attention |

## 🧱 Architecture Overview

- **Input**: Video frames from CAUCAFall Dataset  
- **Preprocessing**: Frame resizing, normalization, data augmentation  
- **Model**:  
  - CNNs with Conv2D, MaxPooling, SE blocks  
  - Spatial & Channel Attention mechanisms  
  - Dense layers with dropout regularization  
- **Output**:  
  - Activity label prediction  
  - Real-time SMS alerts for detected falls

## 🧠 Technologies Used

- 🧠 Deep Learning: CNNs, Attention Mechanisms (SE Blocks, Spatial & Channel)
- 🧮 Frameworks: TensorFlow, Keras
- 🎞️ Dataset: CAUCAFall (includes labeled ADLs and various fall types)
- 🔧 Preprocessing: NumPy, OpenCV
- 📊 Metrics: Accuracy, Precision, Recall, F1-Score
- 🔔 Alert System: Twilio API
- 📦 Deployment: Real-time inference setup

## 📦 Dataset Highlights

- **Name**: CAUCAFall Dataset  
- **Samples**: 5006 videos, 15,901 labeled training frames, 3976 test frames  
- **Activities**: 5 fall types + 5 ADLs  
- **Formats**: .avi (video), .png (frames), .txt (labels)

## 🔍 Future Enhancements

- Real-world dataset expansion
- Privacy-preserving mechanisms
- Deployment on edge devices
- Multimodal sensor fusion
- Improved occlusion handling and camera perspective robustness

## 👩‍💻 Authors

Mogili Greeshma, Mekala Varun, N.V.S Sanjana, Aiswariya Milan K*, Suja Palaniswamy  
Department of Computer Science & Engineering  
Amrita School of Computing, Amrita Vishwa Vidyapeetham, Bengaluru, India  
📩 [Contact Emails]  
- greeshma: bl.en.u4aie22031@bl.students.amrita.edu  
- varun: bl.en.u4aie22037@bl.students.amrita.edu  
- sanjana: bl.en.u4aie22041@bl.students.amrita.edu  
- Aiswariya Milan K: maiswariya@blr.amrita.edu  
- Dr. Suja Palaniswamy: psuja@blr.amrita.edu

---

© 2025 IEEE | 7th International Conference on Intelligent Sustainable Systems (ICISS-2025)  
Licensed for academic and research use only.
