### SwarSetu

**SwarSetu** is a Deep Learning-powered recognition platform designed to bridge communication gaps by interpreting **Sign Language gestures** in real-time. The project utilizes Computer Vision and Convolutional Neural Networks (CNN) to translate hand gestures—representing alphabets, numbers, and common signs—into digital text.

The platform is designed to handle a vast and diverse dataset, ensuring that a wide range of hand gestures are accurately recognized and categorized for seamless interaction.

---

### Features

**Multi-Category Gesture Recognition**
* Identifies a massive range of **49 unique classes**, including the full English alphabet (A-Z), numbers (0-9), and specific gestures like "fist," "paper," "scissors," and "thumbs".
* Processes a large-scale dataset of over **107,000 images**.

**Deep Learning Integration**
* Implements a custom-built **Convolutional Neural Network (CNN)** optimized for image classification.
* Achieves high performance with a **91% training accuracy** and a **96% validation accuracy**.

**Real-Time Image Processing**
* Utilizes a data generator to process images in batches (size 64) with automated resizing to **$64 \times 64$ pixels**.
* Normalizes pixel values for faster and more stable model convergence.

**Scalable Dataset Pipeline**
* Features a robust scanning system that automatically cleans and organizes labels from complex directory structures, ignoring irrelevant folders like 'test' or 'valid'.

---

### Technology Stack

**Development Environment**
* **Google Colab**: Used for high-performance GPU-accelerated training.
* **Google Drive**: Integrated for large-scale dataset storage and management.

**Deep Learning & Machine Learning**
* **TensorFlow / Keras**: The primary framework for building, training, and saving the sequential CNN model.
* **Scikit-Learn**: Used for encoding labels and splitting data into training and validation sets.

**Computer Vision & Data Handling**
* **OpenCV (cv2)**: For real-time image reading, resizing, and preprocessing.
* **NumPy**: For efficient array manipulation and handling image data tensors.

---

### Model Architecture (CNN)

The system uses a `Sequential` model with the following layers to extract and learn gesture patterns:

| Layer Type | Configuration | Purpose |
| :--- | :--- | :--- |
| **Input** | $64 \times 64 \times 3$ | Accepts RGB images of $64 \times 64$ pixels. |
| **Conv2D** | 32, 64, & 128 filters | Extracts features ranging from simple edges to complex gesture shapes. |
| **MaxPooling2D** | $2 \times 2$ | Reduces spatial dimensions to focus on the most important visual features. |
| **Flatten** | 1D Vector | Converts 2D feature maps into a single numerical vector for the learning phase. |
| **Dense** | 128 units (ReLU) | The "thinking" layer that learns patterns between features and labels. |
| **Dropout** | 0.5 (50%) | Prevents overfitting by randomly deactivating neurons during training. |
| **Output** | 49 units (Softmax) | Provides a probability distribution across the 49 possible gesture classes. |

---

### Project Performance

The model was trained iteratively, showing consistent improvement across epochs:
* **Initial Learning:** Started at ~76% accuracy after just 50 steps.
* **Optimization:** Increased to ~88% after further training steps.
* **Final Result:** Concluded with a **96% validation accuracy**, demonstrating high reliability in recognizing unseen gesture data.
