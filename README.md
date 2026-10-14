# 🔬 Electronic Component Classification Using Deep Learning

### Intelligent Electronic Component Recognition with MobileNetV2, TensorFlow and Grad-CAM

**Author:** Leroy Makita Loubaki  
**Project Type:** Personal AI & Computer Vision Project  
**Institution:** ESIGELEC — DARIA Engineering Program

---

## 📖 1. Project Overview

This project focuses on the automatic classification of electronic components using deep learning and computer vision.

The objective is to develop an image classification system capable of identifying different electronic components from photographs.

The solution uses **MobileNetV2**, a convolutional neural network pre-trained on ImageNet, combined with transfer learning and fine-tuning.

A graphical interface allows users to select an image, predict its component category, and visualize the regions influencing the model's decision through heatmaps.

## 🎯 2. Project Objectives

- Develop an image classifier for electronic components.
- Apply transfer learning using MobileNetV2.
- Improve model generalization through data augmentation.
- Evaluate classification performance using accuracy, loss curves and a confusion matrix.
- Build an interactive prediction interface.
- Visualize model attention using Grad-CAM.

## 🛠️ 3. Technologies Used

| Category | Technology |
|---|---|
| Programming | Python |
| Deep Learning | TensorFlow / Keras |
| Neural Network | MobileNetV2 |
| Computer Vision | Image Processing |
| Numerical Computing | NumPy |
| Model Evaluation | Scikit-learn |
| Data Visualization | Matplotlib |
| Graphical Interface | Tkinter |
| Image Processing | Pillow |
| Explainable AI | Grad-CAM |

## 🧠 4. Deep Learning Architecture

The classification model is based on **MobileNetV2**, initialized with ImageNet pre-trained weights.

The original classification head was removed and replaced by a custom classification architecture.

### Model Structure

1. MobileNetV2 feature extractor
2. Global Average Pooling
3. Dense layer with 256 neurons and ReLU activation
4. Dropout layer (0.4)
5. Final classification layer with Softmax activation

### Transfer Learning

Initially, the MobileNetV2 backbone was frozen while training the new classification layers.

A second training phase enabled fine-tuning of the network while keeping its first 100 layers frozen.

## 🖼️ 5. Dataset and Preprocessing

The project uses a directory-organized image dataset containing 16 electronic component categories.

The preprocessing and training configuration includes:

- Input resolution: 128 × 128 pixels
- Batch size: 32
- Training/validation split: 80% / 20%
- Image normalization
- Random rotations
- Zoom augmentation
- Brightness variations

The notebook also includes experimental augmentation utilities such as MixUp and CutMix.

## 📊 6. Experimental Results

The notebook reports the following metrics at the end of the initial training phase:

| Metric | Result |
|---|---:|
| Training Accuracy | 89.74% |
| Validation Accuracy | 92.00% |

These values correspond to the reported training history, not necessarily to the final fine-tuned model or an independent test set.

Additional evaluation of the fine-tuned model is recommended.

## 🔍 7. Classification Examples

The prediction interface displays the predicted component class, confidence score and a visualization heatmap.

Examples from the project include:

| Electronic Component | Prediction Confidence |
|---|---:|
| LCD Display | 98.29% |
| Transistor | 95.76% |
| LED | 95.01% |
| Arduino Board | 88.13% |

These values represent individual prediction confidence scores rather than overall model accuracy.

## 🌡️ 8. Explainable AI — Grad-CAM

Grad-CAM visualization is used to provide visual insights into the model's predictions.

The generated heatmaps highlight image regions contributing to component classification.

This helps analyze how the neural network makes decisions and whether its predictions are influenced by relevant component features.

## 📈 9. Model Evaluation

The project includes:

- Training and validation accuracy curves
- Training and validation loss curves
- A confusion matrix
- Individual prediction confidence scores
- Grad-CAM visualizations

The confusion matrix and validation predictions require alignment verification before drawing detailed class-level conclusions.

## 🖥️ 10. Graphical User Interface

A graphical interface was developed using Tkinter.

The interface enables users to:

1. Select an electronic component image.
2. Load the trained classification model.
3. Display the predicted class.
4. View the prediction confidence.
5. Visualize the model's decision using a heatmap.

## ⚠️ 11. Limitations

- Classification performance depends on dataset quality and diversity.
- Predictions may be affected by lighting, orientation and image backgrounds.
- Similar-looking components can lead to classification errors.
- Additional evaluation on an independent test dataset is needed.
- The reported training metrics should be distinguished from final fine-tuning results.

## 🚀 12. Future Improvements

- Expand the dataset with real-world electronic component images.
- Evaluate performance on an independent test set.
- Improve robustness under different lighting conditions.
- Experiment with additional neural network architectures.
- Optimize inference performance.
- Extend the application toward real-time component recognition.

## 👨‍💻 13. Author

**Leroy Makita Loubaki**

Engineering Student — ESIGELEC, DARIA  
Engineering Apprentice — Constellium

Interested in Artificial Intelligence, Computer Vision, Robotics, Embedded Systems and Industrial Automation.
## 🌐 Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/leroy-makita-loubaki-a78792290/)
[![TikTok](https://img.shields.io/badge/TikTok-Follow-000000?style=for-the-badge&logo=tiktok&logoColor=white)](https://www.tiktok.com/@kingtronix5)
[![YouTube](https://img.shields.io/badge/YouTube-Subscribe-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtube.com/@leroymakitaloubaki)

Feel free to connect with me and explore my engineering, robotics, and artificial intelligence projects.

---

*Personal Deep Learning & Computer Vision Project.*
