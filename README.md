# Brain Tumor Detection with Deep Learning

## Description

This project employs deep learning techniques to classify brain tumors into the following categories:

1. **Glioma Tumor**
2. **Meningioma Tumor**
3. **No Tumor**
4. **Pituitary Tumor**

The project consists of:
- **Dataset exploration and visualization**: Insights into the data used for training and testing.
- **CNN training and evaluation**: Building and training a convolutional neural network (CNN) for classification.
- **GUI application**: An interactive interface for real-time predictions and tumor visualization.

---

## Requirements

### Python Version
- `Python 3.7+`

### Libraries
Install the required libraries using:
```bash
pip install -r requirements.txt
```

Key dependencies include:
- `numpy`
- `opencv-python`
- `tensorflow`
- `matplotlib`
- `PySimpleGUI`
- `Pillow`
- `requests`

---

## Project Structure

```
Brain_Tumor_Detection/
│
├── brain_tumor.ipynb          # Dataset exploration and visualization
├── brain_tumor_cnn.ipynb      # CNN training and evaluation
├── brain_tumor_gui_hlght.ipynb # GUI for predictions and tumor highlighting
├── brain_tumor_model.h5       # Trained CNN model
├── Training/                  # Training data
├── Testing/                   # Testing data
├── requirements.txt           # requirements
└── README.md                  # Project documentation
```

---

## Dataset

The model was trained on the **Brain Tumor MRI Dataset** available on Kaggle:

[Brain Tumor MRI Dataset - Kaggle](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)

The dataset contains MRI images classified into four categories: Glioma Tumor, Meningioma Tumor, No Tumor, and Pituitary Tumor. It is split into training and testing directories with subfolders for each class.

---

## Steps to Run

### 1. Dataset Preparation
- Ensure the dataset is organized as follows:
  ```
  Training/
      Glioma/
      Meningioma/
      No_Tumor/
      Pituitary/
  Testing/
      Glioma/
      Meningioma/
      No_Tumor/
      Pituitary/
  ```

### 2. Train the Model
- Open and run `brain_tumor_cnn.ipynb` to:
  - Load and preprocess the dataset.
  - Train the CNN model.
  - Save the trained model as `brain_tumor_model.h5`.

### 3. Launch the GUI
- Open and run `brain_tumor_gui_hlght.ipynb` to launch the GUI.
- Use the GUI to:
  - Upload images or fetch them from a URL.
  - Predict tumor types and visualize highlighted regions.

---

## Evaluation and Results

### 1. Dataset Insights
Include visuals such as:
- **Class Distribution**: A bar chart showing the number of samples in each class for both training and testing datasets.

### 2. Model Performance
- **Accuracy and Loss Plots**: Display training and validation accuracy/loss over epochs.
- **Confusion Matrix**: Evaluate the classification performance for the testing set.

### 3. GUI Demonstration
Add screenshots showcasing:
- **GUI Interface**: Show the layout and user-friendly design.
- **Prediction Results**: Highlight the tumor type and confidence score.
- **Tumor Highlighting**: Demonstrate how tumor regions are outlined in uploaded images.

---

## Future Work

1. **Tumor Segmentation**
   - Integrate precise segmentation techniques to highlight tumor regions more accurately.

2. **Model Optimization**
   - Experiment with advanced architectures like ResNet or EfficientNet for better accuracy.

3. **Web Deployment**
   - Deploy the model as a web-based application for wider accessibility.

---

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your proposed changes.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.
