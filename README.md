Car Classification Using VGG16
Overview
This project uses transfer learning with the VGG16 model to classify car images into seven categories. It uses TensorFlow/Keras and a car image dataset organized into training and testing folders.
Technologies
- Python
- TensorFlow / Keras
- VGG16 (ImageNet pretrained weights)
- Matplotlib
- Kaggle Notebook
Workflow
1. Load training and test images at 224 × 224 pixels.
2. Preprocess images for VGG16.
3. Fine-tune the later VGG16 layers while freezing earlier layers.
4. Add a classification head with a 512-unit Dense layer, Dropout, and a 7-class softmax output.
5. Train with RMSprop, sparse categorical cross-entropy, and early stopping.
6. Evaluate the model and plot training/validation loss.
How to Run
1. Download or attach the car image dataset with train and test folders.
2. Update the dataset paths in the notebook for your environment.
3. Install the required libraries:
   pip install tensorflow matplotlib
4. Run car-classification-using-vgg16.ipynb in Kaggle or Jupyter Notebook.
Note
The notebook uses the test dataset as validation data during training and evaluates on that same dataset. For a more reliable final evaluation, use a separate validation set and keep the test set for final evaluation.
