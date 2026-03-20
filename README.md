# 🧘 Smart Yoga - AI Yoga Pose Detection & Recommendation System

## 📌 Overview

Smart Yoga is an AI-based application that helps users perform yoga correctly and maintain a healthy lifestyle. It uses computer vision and machine learning to detect yoga poses, recommend suitable exercises, and provide real-time feedback.

This system is designed for both beginners and advanced users to ensure proper posture, avoid injuries, and improve overall wellness.

---

## 🚀 Features

* 🧠 Real-time yoga pose detection using webcam
* 📷 Upload yoga image → detects the pose and shows its details
* 🤖 AI-based pose classification
* 📊 Real-time accuracy score while performing yoga
* 🧘 Personalized yoga recommendations based on user health inputs:

  * Age
  * Gender
  * BMI
  * Disorder
  * Pain level
* ⚡ Fast and efficient performance

---

## 🛠️ Tech Stack

* Python
* OpenCV
* MediaPipe (Pose Estimation)
* Machine Learning / Deep Learning
* NumPy
* Pandas
* Flask

---

## 📂 Project Structure

```
Smart_Yoga/
│── static/
│── templates/
│── models/
│── dataset/
│── app.py / main.py
│── requirements.txt
│── README.md
```

---

Tested 7 different algorithms on our dataset. The **SVM (SVC)** proved to be superior:

- **SVM Accuracy:** 91.51% (Winner)  
- **Neural Network (MLP):** 88.86% (Slower to train)  
- **Random Forest:** 85.94%

---

## The "Specialist" Strategy

To ensure the live webcam feature was fast and accurate, we trained a separate **Specialist Model**.  
While the main model knows 28 classes, the specialist model focuses only on the 9 specific poses used in the live feature.  
This reduced confusion and boosted accuracy to **96.94%**.


## ⚙️ Installation

1. Clone the repository:

```
git clone https://github.com/your-username/Smart_Yoga.git
```

2. Navigate to the project folder:

```
cd Smart_Yoga
```

3. Install dependencies:

```
pip install -r requirements.txt
```

---

## ▶️ Run the Project

```
python app.py
```

Then open in browser:

```
http://localhost:5000
```

---

## 🧠 How It Works

* Captures live video using webcam
* Detects body keypoints using MediaPipe
* Analyzes posture using joint angles
* Classifies yoga poses using ML model
* Provides:

  * Pose name
  * Pose details (for uploaded images)
  * Real-time accuracy score
* Recommends yoga poses based on user health data


## 📊 Future Improvements

* Add more yoga poses
* Improve model accuracy
* Mobile app integration
* Voice-based guidance

---

## 🤝 Contributing

Feel free to fork and contribute to this project.

---

## 📜 License

This project is for educational purposes.

---

## 👩‍💻 Author

**Meezan Mulla**
AI/ML Engineering Student
