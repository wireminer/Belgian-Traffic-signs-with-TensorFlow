# Belgian-Traffic-signs-with-TensorFlow
This project demonstrates how computer vision and deep learning can be applied to real-world image classification tasks
# 🇧🇪 Belgian Traffic Signs Classification with TensorFlow

A deep learning model using Convolutional Neural Networks (CNNs) to classify Belgian road signs. Trained using TensorFlow and Keras.
This notebook uses several technologies and libraries for data analysis, machine learning, and visualization. Here's a summary of the key technologies used:

### **1. Programming Language**
- **Python**: The notebook is written in Python, which is evident from the use of Python libraries and syntax.

### **2. Libraries & Frameworks**
- **TensorFlow (v2.18.0)**: A deep learning framework used for building and training machine learning models, particularly for traffic sign classification.
- **scikit-image (skimage, v0.25.2)**: Used for image processing tasks (e.g., resizing, grayscale conversion).
- **NumPy (v2.0.2)**: A fundamental library for numerical computations in Python.
- **Matplotlib (v3.10.0)**: A plotting library used for visualizing data (e.g., histograms, images).
- **random**: Used for generating random numbers or shuffling data.
- **os**: Used for interacting with the operating system (e.g., file and directory operations).
- **Google Colab**: The notebook appears to be run in Google Colab, as indicated by `drive.mount('/content/drive')`, which mounts Google Drive.

### **3. Data Handling & Visualization**
- **Google Drive Integration**: The notebook mounts Google Drive to access datasets (`/content/drive/MyDrive/Belgian Traffic signs`).
- **Image Processing**:
  - `skimage.io.imread`: For reading images.
  - `skimage.transform.resize`: For resizing images.
  - `rgb2gray`: For converting images to grayscale.
- **Matplotlib (`plt.hist`, `plt.show`)**: For plotting histograms and displaying images.

### **4. Machine Learning & Data Preparation**
- **TensorFlow Operations**:
  - `tf.constant`: For creating tensors.
  - `tf.multiply`: For element-wise multiplication.
- **Data Loading Function (`load_data`)**:
  - Reads `.ppm` image files.
  - Resizes images to a fixed size (32x32 pixels).
  - Organizes images and labels for training.

### **5. Additional Tools**
- **Watermark (`%watermark`)**: A tool to display version information for libraries (TensorFlow, scikit-image, Matplotlib, NumPy, random).
- **File Management**:
  - `os.listdir`, `os.path.isdir`, `os.path.join`: For navigating and loading dataset directories.

### **6. Dataset**
- **Belgian Traffic Signs Dataset**: The notebook loads and processes traffic sign images from the "BelgiumTSC_Training/Training" and "BelgiumTSC_Testing/Testing" directories.

### **Key Workflow Steps**
1. **Mount Google Drive** to access the dataset.
2. **Install and check library versions** (e.g., TensorFlow, scikit-image).
3. **Load and explore the dataset**:
   - Images are resized to 32x32 pixels.
   - Labels are extracted from directory names.
4. **Data Analysis**:
   - Print dimensions of the dataset (`images_array.ndim`, `labels_array.size`).
   - Plot a histogram of label distribution.
5. **TensorFlow Basics**:
   - Demonstrates tensor operations (e.g., `tf.multiply`).
6. **Visualization**:
   - Displays sample images and label distributions.

- Accuracy: 0.903% on test data
