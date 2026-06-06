# 🤟 SignSense


---

## 📌 Overview

SignSense is a computer vision and machine learning project designed to translate sign language gestures into text in real time. The system combines static hand gesture recognition and dynamic gesture recognition to enable continuous sentence formation from sign language inputs.

By leveraging hand landmark tracking, traditional machine learning, and deep learning techniques, SignSense provides an interactive platform for bridging communication gaps and exploring human-computer interaction through sign language recognition.

---

## ✨ Features

- ⚡ Real-time gesture-to-text translation
- 🧠 Hybrid recognition pipeline (Static + Motion)
- ✋ Hand landmark detection using MediaPipe
- 🔤 Recognition of alphabets, numbers, and control gestures
- 🎬 Dynamic word recognition using temporal sequences
- 📝 Continuous sentence generation
- 🔄 Mode switching between static and motion recognition
- ⌨️ Interactive controls for editing generated text

---
## 📸 Demo
<table>
<tr>
<td align="center">
<img src="https://github.com/user-attachments/assets/86522bde-991d-4bf6-8971-179c7eb0b952" width="450">
<br>
<b>Static Gesture Recognition</b>
</td>

<td align="center">
<img src="https://github.com/user-attachments/assets/72dd23f8-6b6b-4863-a4de-b11be5a80b30" width="450">
<br>
<b>Motion Gesture Recognition</b>
</td>
</tr>
</table>

---
## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Python | Core development |
| OpenCV | Video capture and image processing |
| MediaPipe | Hand landmark detection |
| Scikit-learn | Static gesture classification |
| TensorFlow / Keras | LSTM-based motion recognition |
| NumPy | Data processing and feature engineering |

---

## ⚙️ Methodology

### 🟢 Static Gesture Recognition

- MediaPipe extracts **21 hand landmarks**.
- Landmark coordinates are normalized into a **42-dimensional feature vector**.
- A **Random Forest classifier** predicts static gestures such as alphabets, numbers, and control commands.

### 🔵 Motion Gesture Recognition

- Gesture sequences are captured across **30 consecutive frames**.
- Each frame contains normalized hand landmark features.
- An **LSTM network** analyzes temporal patterns to recognize dynamic sign language words.

### 🟣 Hybrid Recognition Pipeline

- Static and motion recognition models operate within a unified framework.
- Users can switch modes depending on the gesture type.
- Predictions are combined to generate meaningful text output in real time.

---

## 🚀 Key Contributions

- Designed the landmark-based feature extraction pipeline.
- Developed the Random Forest classifier for static gesture recognition.
- Built the LSTM-based sequence model for dynamic gesture recognition.
- Integrated both models into a hybrid inference framework.
- Prepared and processed training datasets.
- Evaluated system performance using standard classification metrics.

---

## 🚧 Challenges

- Limited availability of large-scale Indian Sign Language (ISL) datasets.
- Performance sensitivity to lighting conditions and background variations.
- Generalization across different users and hand orientations.

---

## 📈 Future Enhancements

- 🇮🇳 Support for Indian Sign Language (ISL)
- 📸 Larger and more diverse datasets
- 🌐 Web-based deployment
- 🎙️ Speech synthesis integration
- 🤖 Improved sentence prediction and language modeling
- 👤 Enhanced user adaptation and personalization

---

## ▶️ Getting Started

### Clone the Repository

```bash
git clone https://github.com/shivanshh-oo/SignSense.git
cd Signsense-main
```

### Install Dependencies

```bash
pip install opencv-python mediapipe scikit-learn tensorflow numpy jupyter pyttsx3
```

### Run the Project

Open:

```text
Hybrid_inference_classifier.ipynb
```

and click **Run All** to start the real-time gesture recognition system.

---

