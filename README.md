# Plant Species Image Classifier (20 Classes)

This project uses a Convolutional Neural Network (CNN) built with TensorFlow/Keras to classify 20 different species of flowers with **86.20% accuracy**.

## 🔗 Project Link
* **Google Colab Notebook:** [View Project Here](https://colab.research.google.com/drive/1PbjFRL-OjVKxQpNkHv8AFCzJ9Z2rNqxw?usp=sharing)

## 📊 Model Performance
* **Final Validation Accuracy:** 86.20%
* **Final Validation Loss:** 0.49
* **Epochs:** 15

## 📑 Laboratory Reflection & Answers

### 1. Visualization & Overfitting
* **Signs of Overfitting:** Overfitting happens if Training Accuracy keeps going up while Validation Accuracy stays flat or drops. This means the model is just memorizing photos.
* **Effect of Data Augmentation:** It helped the validation accuracy stay high (86.20%) because it forced the model to learn the actual shape of the flowers rather than just one specific photo.

### 2. Model Improvement
* **Purpose of Dropout:** It randomly "turns off" some neurons during training. This prevents the model from relying on "shortcuts" and forces the entire network to learn more effectively.
* **Why Augmentation Improves Generalization:** It creates "new" training images by tilting or zooming the ones you have. This teaches the model that a flower is still the same species even if the camera angle changes.

### 3. Performance Comparison
* **Accuracy Before vs. After:** Before improvements, the model was likely memorizing. After adding Dropout and Augmentation, the model became stable with a strong 86.20% accuracy.
* **Most Helpful Technique:** Data Augmentation was the most helpful because it gave the model the variety it needed to tell the difference between 20 flower types.

### 4. Deployment & Application
* **Importance of Saving:** Saving the model as a `.keras` file stores the AI's "brain." This lets you use it instantly later without waiting 20 minutes to train it again.
* **Real-World Application:** This could be used in a Mobile App for hikers to identify plants in the wild or for gardeners to identify flowers in their backyard.
