## Upgrad Melanoma Detection Assignment (NN) 19March2025 [BalkrishnanV]
========================================================================
# Melanoma Detection Assignment


## Table of Contents
* [General Info](#general-information)
* [Libraries Used](#technologies-used)
* [Melanoma Detection Final Model analysis](#inferences)
* [Acknowledgements](#acknowledgements)

## General Information
**Problem statement**: To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

**The dataset** consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

**The data set contains the following diseases:**

- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

## Libraries Used
- Tensorflow
- Numpy
- Pandas
- Matplotlib
- keras
- keras.losses: SparseCategoricalCrossentropy
- keras.callbacks: ReduceLROnPlateau, EarlyStopping, ModelCheckpoint
- keras.optimizers: Adam
- keras.layers: BatchNormalization, Dense, Dropout, Activation, Flatten, Conv2D, MaxPool2D, Rescaling , RandomZoom, RandomFlip, RandomRotation
- keras.preprocessing.image: ImageDataGenerator
- keras.models: Sequential

## Some inferences from the Melanoma Detection Final Model analysis
![final-model-plots](https://github.com/user-attachments/assets/83a3199f-229a-4686-a97a-47a335870882)

>> Left Plot: Training and Validation Accuracy The training accuracy (blue) increases steadily and reaches above 90%.

>> Left Plot: The validation accuracy (orange) follows a similar trend but has fluctuations, stabilizing around 85%.

>> Left Plot: The gap between training and validation accuracy suggests some overfitting, but it’s not extreme.

>> Right Plot: Training and Validation Loss The training loss (blue) consistently decreases, which is expected.

>> Right Plot: The validation loss (orange) also decreases but fluctuates more.

>> Right Plot: Around epoch 15-20, validation loss stops decreasing significantly, suggesting diminishing returns in training.

>> Good Performance: The model learns well, and validation accuracy is close to training accuracy.

>> Overfitting Risk minimized: The gap between training and validation accuracy suggests overfitting has been minimized.

>> Good Learning Rate: No sudden jumps in loss, meaning the optimizer is working well.

>> Early Stopping Helped: The validation loss is fluctuating, which might indicate a need for early stopping. Hence implemented this in the above solution.


## Acknowledgements
- This project was proposed by [upgrad.com](https://learn.upgrad.com/course/5810/segment/59537/359023/1082443/5402985).

## Contact
Created by [balkrishnan.venkiteswaran@gmail.com] - feel free to contact me!


## License
This project is open source and available under the [MIT License]([https://github.com/balkrishnan/Melanoma_Detection_BalkrishnanV/blob/main/LICENSE].

