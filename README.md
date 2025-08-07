# 🧠 Gender and Age Detection using Deep Learning and OpenCV

This is a Python-based computer vision project that detects human faces in images or video streams and predicts their **gender** and **age group** using deep learning models (Caffe) and OpenCV.

---

## 📌Objective

- Detect faces in real-time using OpenCV’s DNN module.
- Predict **Gender**: Male / Female.
- Predict **Age Group**: One of 8 classes.
- Support both **image files** and **webcam input**.
- Use pretrained deep learning models for accuracy and speed.


## 📖About the Project :

<p>In this Python Project, I had used Deep Learning to accurately identify the gender and age of a person from a single image of a face. I used the models trained by <a href="https://talhassner.github.io/home/projects/Adience/Adience-data.html">Tal Hassner and Gil Levi</a>. The predicted gender may be one of ‘Male’ and ‘Female’, and the predicted age may be one of the following ranges- (0 – 2), (4 – 6), (8 – 12), (15 – 20), (25 – 32), (38 – 43), (48 – 53), (60 – 100) (8 nodes in the final softmax layer). It is very difficult to accurately guess an exact age from a single image because of factors like makeup, lighting, obstructions, and facial expressions. And so, I made this a classification problem instead of making it one of regression.</p>

## 📚Dataset :
<p>For this python project, I had used the Adience dataset; the dataset is available in the public domain and you can find it <a href="https://www.kaggle.com/ttungl/adience-benchmark-gender-and-age-classification">here</a>. This dataset serves as a benchmark for face photos and is inclusive of various real-world imaging conditions like noise, lighting, pose, and appearance. The images have been collected from Flickr albums and distributed under the Creative Commons (CC) license. It has a total of 26,580 photos of 2,284 subjects in eight age ranges (as mentioned above) and is about 1GB in size. The models I used had been trained on this dataset.</p>

---

## 🐍Additional Python Libraries Required :
<ul>
  <li>OpenCV</li>
  
       pip install opencv-python
</ul>
<ul>
 <li>argparse</li>
  
       pip install argparse
</ul>

---

## 📦 Download All Pre-trained Model Files

To run this project, you'll need to download the required pre-trained models for face, age, and gender detection.

🎯 **Click the link below to download all required model files:**  
👉 [Download Model Files Folder (Google Drive)](https://drive.google.com/drive/folders/1VdHqNUjTo4_bjIWBPf4RiswgzL5puA2l?usp=drive_link)

📁 **This folder includes:**
- `age_deploy.prototxt`
- `age_net.caffemodel`
- `gender_deploy.prototxt`
- `gender_net.caffemodel`
- `opencv_face_detector.pbtxt`
- `opencv_face_detector_uint8.pb`

> 📌 **Instructions**: Download all the files from the folder and place them in the same directory as your `detect.py` script.

---

## ✨ Features

- ✅ Face detection using Haarcascade or DNN-based face detector.
- ✅ Gender classification using a pre-trained Caffe model.
- ✅ Age classification into the following 8 groups:
  - 0–2
  - 4–6
  - 8–12
  - 15–20
  - 25–32
  - 38–43
  - 48–53
  - 60–100
- ✅ Command-line arguments for custom images.
- ✅ Webcam support for real-time predictions.

---

## 🚀 Usage

<ul>
  <li>📷 Predict from Image</li>
  
       python detect.py --image man2.jpg
</ul>
<ul>
 <li>🎥 Predict from Webcam</li>
  
       python detect.py
</ul>

**📌** Press Esc to stop webcam mode.

---

## 🖼️ Demo

<p><b>NOTE:- I downloaded the images from Google,if you have any query or problem i can remove them, i just used it for Educational purpose.</b></p>

    >python detect.py --image man2.jpg
    Gender: Male
    Age: 25-32 years
    
<img width="1244" height="863" alt="Screenshot 2025-08-05 071900" src="https://github.com/user-attachments/assets/2f33066d-7bd3-40b0-810e-dda8a854a194" />


    >python detect.py --image kid2.jpg
    Gender: Female
    Age: 4-6 years
    
<img width="991" height="888" alt="Screenshot 2025-08-05 071820" src="https://github.com/user-attachments/assets/a38a2bb0-ae8a-46ea-abcf-db561abc108a" />

---

## 🗂 Project Structure

<img width="388" height="407" alt="image" src="https://github.com/user-attachments/assets/10694873-ebf4-45f4-89da-b904044c6fce" />
