# Face Mask Detection using Deep Learning

## Project Overview

This project implements a face mask detection system using computer vision and deep learning techniques. The system is capable of identifying whether a person is wearing a face mask or not from images, video files, and real-time webcam input. It uses a convolutional neural network based on MobileNetV2 for classification and OpenCV for face detection.

The goal of this project is to demonstrate the application of deep learning in a real-world scenario, specifically in public health monitoring and safety compliance.

---

## Features

* Detects whether a person is wearing a mask or not
* Supports image, video, and real-time webcam input
* Uses a pre-trained deep learning model (MobileNetV2)
* Provides performance evaluation using metrics such as accuracy, confusion matrix, precision, recall, and F1-score
* Modular code structure for easy understanding and extension

---

## Technologies Used

* Python
* OpenCV
* TensorFlow / Keras
* NumPy
* Matplotlib
* Scikit-learn

---

## Project Structure

```bash
face-mask-detector/
│── dataset/
│   ├── with_mask/
│   └── without_mask/
│
│── test_images/
│   └── test.jpg
│
│── models/
│   └── mask_detector.keras
│
│── train.py
│── detect_image.py
│── detect_video.py
│── detect_webcam.py
│
│── requirements.txt
│── README.md
│── report.pdf
```

---

## Dataset

The dataset consists of two categories:

* with_mask
* without_mask

Download the dataset from the following link:
https://www.kaggle.com/datasets/omkargurav/face-mask-dataset

Note: The dataset is not included in this repository due to its size. After downloading, extract it and place it in the project directory following the structure shown above.

---

## Installation and Setup

### Step 1: Clone the Repository

```bash
git clone <your-repository-link>
cd face-mask-detector
```

### Step 2: Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Usage

### Train the Model

```bash
python train.py
```

This will train the model on the dataset and save it in the `models/` directory.

---

### Run Detection on an Image

```bash
python detect_image.py
```

Make sure the image path is correctly set inside the script.

---

### Run Detection on a Video

```bash
python detect_video.py
```

---

### Run Real-Time Webcam Detection

```bash
python detect_webcam.py
```

---

## Evaluation Metrics

The model is evaluated using the following metrics:

* Accuracy
* Confusion Matrix
* Precision
* Recall
* F1 Score

These metrics help in understanding the performance of the classification model on unseen data.

---

## Results

The model achieves high accuracy on the validation dataset (approximately 90–95%, depending on dataset quality). The system is capable of detecting faces and classifying mask usage in real time.

---

## Limitations

* Face detection using Haar Cascade may not perform well in all conditions, especially with occlusions or low lighting
* Performance depends on the diversity and quality of the dataset
* May not generalize well to all real-world scenarios without further training

---

## Future Improvements

* Replace Haar Cascade with more advanced face detection models such as YOLO or SSD
* Deploy the model as a web application using Flask or Django
* Improve accuracy using a larger and more diverse dataset
* Optimize for mobile or edge devices

---

## Author

Your Name



## License

This project is intended for educational purposes only.

