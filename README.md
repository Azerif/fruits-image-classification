# Image Classification Project: Fruits Classification 🍇

This project aims to classify fruit images using a deep learning model based on MobileNetV2. The dataset used is sourced from [Kaggle](https://www.kaggle.com/datasets/utkarshsaxenadn/fruits-classification).

## Project Steps

### 1. Data Preparation
- The dataset was downloaded from Kaggle and extracted.
- Data from the `train`, `test`, and `valid` folders were combined into a single dataset folder.
- Data augmentation was performed to increase the variety of training data.

### 2. Data Processing
- The data was split into three sets: `train`, `val`, and `test` with proportions of 80:10:10.
- Data augmentation was applied using transformations such as rotation, flipping, and brightness/contrast adjustments.

### 3. Model Training
- MobileNetV2 was used as the base model with transfer learning.
- The model was trained using a data generator with augmentation.
- Callbacks were used to save the best model and stop training if the validation accuracy reached the target.

### 4. Evaluation and Visualization
- Accuracy and loss during training were visualized.
- The model was evaluated on the test data to calculate the final accuracy.

### 5. Model Conversion
- The best model was converted to the SavedModel and TFLite formats.
- Class labels were saved in a `label.txt` file for inference.

### 6. Inference
- The TFLite model was used to make predictions on new images.
- Class probabilities were visualized alongside the input images.

## How to Run the Project

1. **Set Up the Environment**
   - Ensure Python 3.7+ is installed.
   - Install dependencies using the command:
     ```bash
     pip install -r requirements.txt
     ```

2. **Run the Notebook**
   - Open and run `notebook.ipynb` to train the model, evaluate it, and perform inference.

3. **Inference with TFLite**
   - Use the TFLite model for predictions by running the `predict_tflite` function in the notebook.

## Final Results
- **Validation Accuracy:** ~95%  
- **Test Accuracy:** ~95%  
- The trained model can classify fruit images with high accuracy.





# fruits-image-classification
