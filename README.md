# Facial-Similarity-of-YouTube-Influencers-using-Machine-Learning

Datasets

The YouTube Faces Database is used for training the Siamese Neural Networks and can be downloaded from https://www.cs.tau.ac.il/~wolf/ytfaces/

The influencer data, which is manually collected, includes images of 15 (10 males and 5 females) YouTube influencers. This dataset is only used for evaluating the models. The influencer data can be found in this repository.

Notebook files

Each notebook contains 2 Siamese Neural Networks architectures. The networks are trained on 2, 10 or 30 images from the YouTube Faces data. Please make sure that your training directory contains only names with images inside that directory. 

The files are named as follows for the uncropped (without face detection) networks: SiameseYoutube + amount of training images. 

The files are named as follows for the cropped (with face detection) networks: SiameseYoutube + amount of training images + name of face detection algorithm. Where 'name of face detection algorithm' is either Haar (Haar cascade classifier) or Dlib (Dlib Convolutional Neural Network). 

Packages and versions

The programming part of this research is implemented with Python 3.8.5. A separate environment was created within Anaconda Navigator, where Juypyter Notebook was mainly used for developing Python code. The code depends on the following packages with their versions: PyTorch (1.10.2) with CUDA toolkit (11.3.1), Matplotlib (3.5.1), Numpy (1.21.5), OpenCV (4.0.1), deepface (https://github.com/serengil/deepface) and scikit learn (0.23.2).
