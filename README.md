# 🧠 Handwritten Digit Classification with ResNet-Style CNN on MNIST

This project implements a **ResNet-inspired Convolutional Neural Network (CNN)** to classify handwritten digits using the **MNIST dataset**. It uses TensorFlow and Keras to build, train, and evaluate the model.

---

## 📁 Project Structure

- `model.py`: Contains the complete code for data loading, model building, training, and evaluation.
- `README.md`: This file.

---

## 📦 Dependencies

- Python 3.7+
- TensorFlow 2.x

Install dependencies using:

```bash
pip install tensorflow
📊 Dataset
The MNIST dataset consists of:

60,000 training images

10,000 testing images

Each image: 28x28 pixels (grayscale)

Keras provides the dataset out-of-the-box via tf.keras.datasets.mnist.

🧱 Model Architecture
This CNN includes:

Initial convolution layer with ReLU and batch normalization

3 Residual blocks:

Two with identity skip connections

One with downsampling (stride 2)

Global average pooling

Final dense layer with softmax activation

🔁 Residual Blocks:
Residual connections help mitigate the vanishing gradient problem and improve performance for deeper networks.

🏋️‍♂️ Training Details
Optimizer: Adam

Loss: Categorical Crossentropy

Metrics: Accuracy

Epochs: 5

Batch size: 64

Validation split: 10%
