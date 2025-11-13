# 🐱🐶 Cats vs Dogs Image Classifier

This project is part of the **Machine Learning with Python** certification by [freeCodeCamp.org](https://www.freecodecamp.org/).  
The goal is to create a convolutional neural network (CNN) that classifies images of cats and dogs with at least **63% accuracy**.

---

## 🎯 Objective

- Build a CNN using **TensorFlow 2.x** and **Keras**.
- Use data augmentation to prevent overfitting.
- Train the model on **2,000 training images** and validate on **1,000 images**.
- Test the model on 50 unlabeled images and predict cats or dogs.

---

## 🧠 Approach

1. **Preprocessing:**
   - Rescale image pixel values from `[0, 255]` → `[0, 1]`.
   - Apply data augmentation (rotation, width/height shift, zoom, horizontal flip).

2. **Model Architecture:**
   - Convolutional layers with ReLU activations.
   - MaxPooling layers for downsampling.
   - Fully connected (Dense) layer with dropout.
   - Sigmoid activation for binary classification.

3. **Training:**
   - Loss function: `binary_crossentropy`
   - Optimizer: `adam`
   - Metrics: `accuracy`
   - Epochs: 15
   - Batch size: 128

---

## 🧩 Project Structure

cats-vs-dogs-classifier/
│
├── cats_and_dogs/ # Dataset folder (train, validation, test)
├── cats_dogs_classifier.ipynb # Main Colab notebook
└── README.md # Project documentation


---

## 📊 Results

- Model accuracy on validation set: **>63%**  
- Predictions on test images show cats vs dogs with probabilities.

---

## 📤 How to Run

1. Open `cats_dogs_classifier.ipynb` in **Google Colab**.  
2. Run each cell sequentially.  
3. After training, the model will display test images with predicted labels.  
4. To submit on freeCodeCamp:
   - Click **File → Save a copy in Drive**
   - Share the notebook with **anyone with the link**.
