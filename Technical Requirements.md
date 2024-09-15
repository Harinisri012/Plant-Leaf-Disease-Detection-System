# Plant Leaf Disease Detection System

## **Technical Specifications**

### 1. **Programming Language:**
   - Python 3.12.0

### 2. **Libraries and Frameworks:**
   - **TensorFlow/Keras**: Used for building and training both the CNN and VGG16 models.
   - **OpenCV**: For image processing and augmentation techniques.
   - **Matplotlib/Seaborn**: Used for visualizing model performance, such as accuracy and loss curves.
   - **NumPy**: For numerical operations and array handling.
   - **Pandas**: For data manipulation and loading structured data.
   - **scikit-learn**: Used for splitting data and evaluating models with classification metrics.

### 3. **Model Architectures:**
   - **Basic CNN**: Custom-built Convolutional Neural Network with multiple convolutional, pooling, and dense layers.
   - **VGG16 (Transfer Learning)**: Pre-trained VGG16 model (ImageNet weights) with custom fully connected layers for plant disease classification.

### 4. **Dataset:**
   - **Plant Leaf Images**: A small dataset with images of leaves in three categories:
     - Healthy
     - Powdery mildew
     - Rust
   - **Dataset Structure**:
     - Split into training, validation, and testing sets.
     - Data augmentation applied to increase the dataset size.

### 5. **Hardware Requirements:**
   - **CPU-Based System**: The project was designed to run on a system without a GPU, utilizing smaller architectures to fit within hardware limitations.
   - **RAM**: At least 8GB of RAM is recommended due to model and data processing.
   - **Storage**: The dataset is small, requiring minimal disk space (< 1 GB).

### 6. **Key Functions:**
   - **Data Preprocessing**: Resizing, normalization, and augmentation of images.
   - **Model Training**: Both CNN and VGG16 models are trained using `categorical_crossentropy` as the loss function and `Adam` as the optimizer.
   - **Model Evaluation**: Accuracy and loss evaluated on the test set, with visualizations generated for comparison.

### 7. **Performance Comparison:**
   - **CNN Model**: Achieved an accuracy of 88.6% on the test dataset.
   - **VGG16 Model**: Achieved an accuracy of 86.0% on the test dataset.
   - The custom CNN performed slightly better due to its simpler architecture, making it more suitable for the small dataset.

---

By following the above technical specifications, the project is designed to be efficient, easy to train on limited hardware, and highly adaptable for plant disease detection tasks.
