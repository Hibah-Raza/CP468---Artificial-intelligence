# CP468 - Artificial Intelligence Group Project

## Intructions on Downloading, Configuring, and Training Our Model + 3 Pre-Trained Models

### 1. Just Run the Imports:)
- Since we already uploaded our ipython notebook for you all you have to do is run the imports and you will be able to run the 2 gradio interfaces and the opencv. Enjoy! 

### *(To be able to run everything yourself, read the steps below!)*

### 2. Download Dataset
- Download the dataset from Kaggle, You need to be signed into Kaggle to download the dataset, so it is highly suggested to create an account before attempting to download it.
- [FER2013 Dataset](https://www.kaggle.com/datasets/msambare/fer2013)

### 3. Extract and Prepare the Dataset
- Once downloaded, extract the zip file and rename the extracted folder to `fer2013`.
- Use your preferred IDE for installation and imports. We used Jupyter Notebook for fast training and validation.
- Install TensorFlow and Gradio by running the following commands:
  ```sh
  !pip install tensorflow
  !pip install gradio
  ```

### 4. Import Libraries and Prepare Data
- Import any other necessary libraries.
- Start by running our generators for validation and training data. After doing so, you should get an output that says:
```sh
Found 28907 images belonging to 7 classes.
Found 7178 images belonging to 7 classes.
```

These are the images inside the train and test folders of the fer2013 file.

### 5. Create a Custom CNN Model
- Create a custom CNN model (which we have already done for you).
- You need 2 datasets that will flow from the directory: one for training and one for validation/test.
- Define your CNN model and add multiple layers to it. After compiling the model, train it.

### 6. Save the Model and Its Weights
- Save your model and its weights. This is necessary when you create an interface for your model to be tested on.
- Optionally, create a graph that displays your training and validation accuracy and loss.

### 7. Use 3 Pre-Trained Models
- Start by importing the pre-trained models.
- Get the weights of the pre-trained models, which will be used for transfer learning with our custom CNN model.
- Define the base model of the pre-trained models without their weights.

### 8. Load Weights and Customize Pre-Trained Models
- Load the weights from either your Google Drive (if using Google Colab) or from your local file (if using Jupyter Notebook). Alternatively, define the weights from ImageNet
- Freeze the layers of the pre-trained models and add custom layers to them.

### 9. Compile and Train Pre-Trained Models
- Compile the pre-trained models and train them for a maximum of 20 epochs.
- Create a Gradio interface for these pre-trained models to test how well they perform on your custom CNN model and dataset.

### 10. Finalize Your Model
- After completing these steps, your custom CNN model and the 3 pre-trained models will be trained on your dataset and ready for use.
