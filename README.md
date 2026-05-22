# Driver Drowsiness Detection System

A real-time driver safety monitoring system using CNN-based computer vision models to detect drowsiness and trigger instant alerts.

---

## Inspiration

This project was inspired by a real-life accident involving my father caused by drowsiness while driving. The goal was to explore how computer vision and deep learning could help improve driver safety through real-time monitoring.

---

## Problem Statement

Driver fatigue is one of the major causes of road accidents worldwide.

Existing solutions are often:
- expensive
- inaccessible
- dependent on advanced hardware

This project explores a lightweight real-time monitoring approach using computer vision and CNN models.

---

## Features

- Real-time drowsiness detection
- Live webcam monitoring
- Eye-state detection
- Facial landmark tracking
- Instant alert triggering
- CNN-based prediction system

---

## Tech Stack

- Python
- OpenCV
- TensorFlow
- CNN
- NumPy
- Computer Vision

---

## Detection Pipeline

```txt
Webcam Feed
      ↓
Frame Extraction
      ↓
Face Detection
      ↓
Eye Region Extraction
      ↓
CNN Prediction
      ↓
Alert Trigger
```

---

## AI Workflow

### Computer Vision Pipeline
- Live webcam frame processing
- Facial landmark tracking
- Eye-region extraction

### CNN Model
Used CNN-based deep learning models for:
- eye-state classification
- fatigue prediction

---

## Performance

- Achieved ~87% detection accuracy
- Optimized for real-time responsiveness
- Designed for continuous monitoring scenarios

---

## Challenges Faced

### Lighting Conditions
Different lighting environments affected detection accuracy.

### False Positives
Balancing sensitivity with reliability.

### Real-Time Processing
Optimizing inference speed while maintaining accuracy.

---

## Learnings

- Real-time ML system design
- CNN implementation for computer vision
- Tradeoffs between accuracy and performance
- Video processing pipeline optimization

---

## Research Publication

Presented research paper:
"Driver Drowsiness Detection System using DL models"

ICDAM-2023 Conference

---

## Future Scope

- Integration with automobile systems
- Multi-sensor driver monitoring
- Advanced fatigue analytics
- Edge-device optimization
- Fleet safety applications

---

## Screenshots

Without Specs
<img width="400" height="711" alt="without_specs" src="https://github.com/user-attachments/assets/5a923f34-e2a2-4895-ba1a-049332cd5f40" />
With Specs
<img width="400" height="711" alt="with_specs" src="https://github.com/user-attachments/assets/345bcc65-8c0d-42a0-b913-9a8d6424874f" />


---

## Github

Repository: https://github.com/kiddo2507/Drowsiness-detection-using-CNN

Dataset taken from http://mrl.cs.vsb.cz/eyedataset

Once the dataset is downloaded, update the directory's path in ```data_splitting.ipynb```. Once the dataset is splitted into open and close, manually split the data into 90:10 training: testing directories. 

Run the ```model_training.ipynb``` file and change the directory's path of ```/models/model.h5```. Let the model train itself. Personally in my Lenovo Thinkpad T470, i7 processor, 16GB RAM it approximately took 85 minutes to run 5 epoches. 

My model is giving an accuracy of 93.94% after final epoch of 5/5. 

Average of accuracy for all the epochs, i.e., the accuracy of the InceptionV3 model is 93.294% and the final loss of the model came out to be 18.11%.

I even tried using ResNet50 for training the model and The average accuracy and loss after using ResNet50 neural network architecture was 50.484% and 69.312% respectively. You can see this work in ```resnet_model_training.ipynb``` file and see all the layers of it in ```resnet_output.txt```.

Once the model is trained, go to ```main.ipynb``` file, make necessary changes in the directory path and run the code. It should be working with 
