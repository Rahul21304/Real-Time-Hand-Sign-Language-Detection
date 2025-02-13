
#  Real-Time-Hand-Sign-Language-Detection

## 📌 Project Overview  
This project implements a **hand gesture recognition system** using **OpenCV, MediaPipe, and an LSTM-based deep learning model**. The system detects hand landmarks, extracts keypoints, and classifies gestures using a trained LSTM model.  

## 🚀 Features  
- **Hand landmark detection** using MediaPipe  
- **Real-time gesture recognition** with OpenCV  
- **LSTM deep learning model** for accurate classification  
- **Dataset collection & preprocessing** for training  
- **Custom visualization** of recognition results  

## 🛠️ Project Structure  
```bash
├── app.py          # Main application for real-time gesture recognition
├── trainmodel.py   # Model training script using LSTM
├── collectdata.py  # Script for collecting images of hand gestures
├── data.py         # Data collection and preprocessing
├── function.py     # Utility functions for hand tracking & feature extraction
├── model.json      # Saved model architecture
├── model.h5        # Trained model weights
└── README.md       # Project documentation
```    

## 📦 Dependencies  
Make sure to install the required dependencies before running the project:  
```bash
pip install numpy opencv-python mediapipe tensorflow scikit-learn
```  

## 📊 Dataset Collection  
- **Image Collection:**  
  - Run `collectdata.py` to collect images of different hand gestures and store them in the `Image/` directory.  
  - Press the corresponding **letter key (A-Z)** to save images for that specific gesture.  

- **Keypoint Extraction:**  
  - The `data.py` script processes collected images and extracts hand keypoints using MediaPipe.  
  - The extracted keypoints are saved as `.npy` files for training.  

## 🏗️ Model Training  
- Run `trainmodel.py` to train an LSTM model on the extracted data.  
- The trained model is saved as `model.h5` and `model.json`.  

## ▶️ Running the Gesture Recognition  
To start real-time gesture recognition, run:  
```bash
python app.py
```  

## 🔗 Future Improvements  
- Expand the dataset with more gestures  
- Improve accuracy with hyperparameter tuning  
- Deploy as a web or mobile app  
