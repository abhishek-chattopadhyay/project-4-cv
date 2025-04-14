# Fractured, Or Not-fractured, That Is The Question
## An image processing and computer vision project at Ironhack

# Intoduction
Computer vision is an interesting application of deep learning. It can be used to classify images among different categories. In this project, I have used computer vision to classify healthy and fractured bones from a pool of X-ray images. The X-ray images contain fractured and non-fractured bones from different parts of the body. The main idea was to apply a deep learning computer vision algorithm to classify them into two categories.

# Project Goals
- Divide the image dataset into train, test and validation data.
- Use data augmentation technique to ampifly the test data e.g rotating or flipping the images.
- Use state-of-the-art computer vision model to predict the outcome. This is an example of transfer learning.
- Calculate the accuracy of the model used
- Presentation to stakeholder

# Data Sources
- [Bone Fractures](https://drive.google.com/file/d/1WeuxOenviI1_ElW5ISED4MhvR_YFYdmB/view?usp=drive_link): The dataset includes multi-region X-ray images focused on diagnosing bone fractures.

# Methodology
- After the dataset is divided into train, test and validation folder, corrupted images have been removed using `Tensorflow`.
- `MobileNetV2` model was used as a computer vision model.
- Training and Testing accuracy and loss function have been calculated for 30 epochs.
- The best model has been saved as `best_model.keras`.

# Key Insights
- `MobileNetV2` works well with an accuracy score of 0.96.
- Type 1 and type 2 errors are very small as can be seen in the confusion matrix.

# Project Structure



# Getting Started



# Extra Notes