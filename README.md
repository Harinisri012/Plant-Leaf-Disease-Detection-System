# Plant-Leaf-Disease-Detection-System

## **Objective:**
The objective of this project is to develop a **Plant Leaf Disease Detection System** utilizing AI models to identify and classify plant leaf diseases based on image data. Early detection of plant diseases is crucial for agricultural sustainability, helping farmers prevent the spread of diseases and ensuring higher crop yields and quality.

## **Steps Involved:**

1. **Data Collection and Preprocessing**:
   - Gathered a small dataset of plant leaf images with three categories: healthy, powdery mildew, and rust.
   - Split the dataset into training, testing, and validation sets.
   - Applied necessary image preprocessing techniques such as resizing, normalization, and augmentation to prepare the data for model training.

2. **Building the Models**:
   - **Basic CNN Model**: Designed a custom Convolutional Neural Network (CNN) with multiple convolutional and pooling layers, followed by fully connected layers and a softmax output for classification.
   - **VGG16 Transfer Learning**: Utilized the pre-trained VGG16 model with ImageNet weights and added custom layers for classification. The base layers of VGG16 were frozen to prevent retraining, and additional dense layers were added for the plant leaf classification task.

3. **Training the Models**:
   - Trained both the **CNN** and **VGG16** models using the training dataset.
   - Used categorical cross-entropy loss and Adam optimizer for both models.
   - Monitored the models' performance by tracking accuracy and loss on the validation dataset.

4. **Evaluation**:
   - Evaluated both models on the test dataset to assess their performance in terms of accuracy and loss.

5. **Comparison of Models**:
   - Compared the performance of the basic CNN model and the VGG16 model on the test set.

## **Comparison:**

| **Model**  | **Accuracy** | **Observation**                                  |
|------------|--------------|--------------------------------------------------|
| **CNN**    | 0.886        | The custom CNN model showed slightly better performance, achieving an accuracy of 88.6%. It performed well due to its simplicity and the dataset size. |
| **VGG16**  | 0.860        | The VGG16 model, while being a powerful transfer learning model, achieved a slightly lower accuracy of 86.0%. This might be due to the small dataset size, where pre-trained models can sometimes overfit or struggle without sufficient fine-tuning. |

## **Conclusion**:
- Both models performed well in classifying the plant leaf images. The custom CNN achieved a higher accuracy (88.6%) compared to VGG16 (86.0%).
- The CNN model's simplicity allowed it to better adapt to the dataset, while the VGG16 model might benefit from further fine-tuning or additional data.

