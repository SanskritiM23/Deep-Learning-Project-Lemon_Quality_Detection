# Deep-Learning-Project-Lemon_Quality_Detection
Developed a lemon quality dataset classifier incorporating cutting edge CNN architecture and image augmentation methodologies.

Lemon dataset has been prepared to investigate the possibilities to tackle the issue of fruit quality control. It contains 2.533 images (300 x 300 pixels). Lemon images are taken on a concrete surface. Dataset also includes empty images of this surface.

Dataset contains images of both bad and good quality lemons under slightly different lighting conditions (all under daylight) and sizes.
Some samples

![Image Description](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRvKP_cgBD37hbQdhCxIqaZtYnZmCkYxg1hFw&usqp=CAU)


### Dataset Handling:
- Utilizes the `tf.keras.preprocessing.image_dataset_from_directory` function to load the dataset.
- Resizes images to a specified size and batches them for efficient processing.

### Dataset Splitting:
- Implements a function `split_dataset()` to split the dataset into training, testing, and validation sets.
- Allows customization of split ratios and shuffling.

### Data Augmentation:
- Incorporates data augmentation techniques like random flipping and rotation to enhance model generalization.

### Model Architecture:
- Constructs a Convolutional Neural Network (CNN) using TensorFlow's Sequential API.
- Employs several convolutional and pooling layers followed by fully connected layers for classification.

### Model Compilation:
- Compiles the model with appropriate loss function, optimizer, and evaluation metrics.

### Model Training:
- Trains the model on the training dataset, validating it on a separate validation set.
- Monitors training progress through epochs, tracking accuracy and loss metrics.

### Model Evaluation:
- Evaluates the trained model on the test dataset to assess its performance.

### Visualization:
- Utilizes Matplotlib to visualize training and validation accuracy/loss trends over epochs.

### Model Saving:
- Saves the trained model in the HDF5 format for future use.


