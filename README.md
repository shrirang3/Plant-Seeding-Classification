
# Plant-Seeding-Classification


Image classification has emerged as one of the key challenges that machine learning (ML) and deep learning (DL) techniques can effectively address. In this project, I will leverage a dataset from a Kaggle competition, which contains images of approximately 960 distinct plant species, spanning 12 different categories, captured at various stages of growth. The images are annotated and presented in RGB format, with a physical resolution of approximately 10 pixels per millimeter. This dataset, provided by the Signal Processing Group of the Department of Engineering at Aarhus University, was made available to the public to stimulate research and development in image recognition and to foster collaboration and idea exchange within the community.

The goal of this project is to utilize ML and DL methodologies to accurately classify and differentiate between these two groups of plants, helping to advance agricultural technologies.


## Dataset

The dataset used in this project is publicly available on Kaggle, originally provided by the Signal Processing Group from the Department of Engineering at Aarhus University, in collaboration with the University of Southern Denmark. The dataset can be accessed here:

https://vision.eng.au.dk/?download=/data/WeedData/NonsegmentedV2.zip

The dataset was collected at Aarhus University's Flakkebjerg Research Station, as part of a collaboration with the University of Southern Denmark. It consists of around 1.7 GB of training data, specifically containing non-segmented images of individual plants. The challenge presented by this dataset lies in the subtle similarities between weed seedlings and crop seedlings, making it difficult to distinguish between them visually.



## Model Architectures and Training Approaches

Model 1: Baseline Convolutional Model with Batch Normalization
This model employs a sequential architecture with convolutional layers followed by activation functions, batch normalization layers, and pooling. The batch normalization helps in stabilizing the training process by normalizing the inputs to each layer, while the pooling layers reduce the dimensionality and prevent overfitting.

Model 2: Convolutional Model with Dropout for Regularization
To experiment with alternative regularization techniques, batch normalization was replaced with dropout layers. Dropout is applied to randomly deactivate neurons during training, which helps mitigate overfitting by making the network less sensitive to specific neuron weights.

Model 3: Model Trained with Data Augmentation
Data augmentation techniques were introduced in this model to improve generalization and robustness. Augmentations such as random rotations, flips, and zooms were applied to artificially increase the diversity of the training data, allowing the model to better capture variations in plant seedling appearances.

Model 4: Class Imbalance Handling Using Augmentor
This model specifically addresses the issue of class imbalance by utilizing the Augmentor Python package. Augmentor was used to generate synthetic samples for the underrepresented classes, ensuring the model had a more balanced dataset during training. This approach enhances the model's ability to classify minority classes more accurately. Refer documentation: https://augmentor.readthedocs.io/en/master/userguide/mainfeatures.html













