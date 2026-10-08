# Facial Emotion Recognition

## Overview
This project aims to detect and classify human facial emotions from images using Convolutional Neural Networks (CNN) and Deep Learning techniques. The system analyzes facial features to identify different emotional states, with applications in human-robot interaction, intelligent marketing, and mental health monitoring.

## Author
**Maryam Taheri Emami**
*Bachelor of Science in Computer Engineering*
National University of Skill, Gorgan Girls' Branch
*Supervisor: Komeil Shahvari*
*June 2025*

## Dataset
The model is trained and evaluated on the **FER-2013** dataset, a widely used benchmark in facial emotion recognition.
*   Contains over 35,000 grayscale images (48x48 pixels).
*   Categorized into 7 distinct emotions: Angry, Disgust, Fear, Happy, Sad, Surprise, and Neutral.

## Methodology & Model Architecture
*   **Preprocessing:** Images are resized (48x48), normalized (scaled 0-1), and augmented (rotation, shifting, zooming, horizontal flip) to improve model generalization.
*   **Network Architecture:** A custom CNN model consisting of multiple Conv2D layers, MaxPooling2D layers, Batch Normalization, Dropout layers, and Dense layers.
*   **Optimization:** Used Nadam optimizer, Early Stopping, ReduceLROnPlateau, and He Normal initialization to improve convergence and prevent overfitting.
*   **Training:** Utilized `ImageDataGenerator` for real-time data augmentation during training.

## Results
*   **Overall Accuracy:** The model achieved an accuracy of approximately **82-83%** on the validation set.
*   **Performance Analysis:** The model showed strong performance in identifying certain emotions (e.g., Class 0 or "Happy"), while classes with similar visual features (e.g., Class 1 and Class 2) had slightly lower accuracy, as indicated by the confusion matrix.
*   **Generalization:** Training and validation loss curves indicate the model is well-fitted without severe overfitting.

## Project Structure
*   `fer_py.ipynb`: Jupyter Notebook containing the Python code for data preprocessing, model building, training, and evaluation.
*   `m-t-1.pdf`: Full project documentation and thesis report.
*   `train.zip` / `Train 2.zip` / `Train 3.zip`: Training datasets (FER-2013).
*   `test.zip`: Test dataset.

## Future Improvements
*   Increasing the dataset size and diversity.
*   Implementing more advanced architectures (e.g., Transfer Learning with ResNet, VGG16).
*   Utilizing K-fold Cross-Validation for more robust evaluation.
*   Addressing class imbalance using data augmentation or class weighting.

## Keywords
Deep Learning, Image Processing, Facial Emotion Recognition, CNN, FER-2013
