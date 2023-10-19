# USPS K-Neigh90: Achieving 90%+ Accuracy with K-Neighbors Classifier over USPS Dataset

**Goal:** Try to build a classifier for the USPS dataset that achieves over 90% accuracy over the test set using K - Neighbors classifier.

Your submission should include the following:
1. cross validation results
2. confusion matrix
3. precision and recall
4. change different K for KNN
5. use different image feature extraction method such as SIFT can add extra credit

**Dataset**: 

USPS： [https://www.kaggle.com/bistaumanga/usps-dataset](https://www.kaggle.com/datasets/bistaumanga/usps-dataset)

USPS contains handwritten digits. It has 7291 train and 2007 test images. The images are 16*16 grayscale pixels.
The dataset is given in hdf5 file format, the hdf5 file has two groups train and test and each group has two datasets: data and target.

Use this code to read the file:



with h5py.File(path, 'r') as hf:

     train = hf.get('train')
     
     X_train = train.get('data')[:]
     
     y_train = train.get('target')[:]
     
     test = hf.get('test')
     
     X_test = test.get('data')[:]
     
     y_test = test.get('target')[:]

 
**Code example:**
[https://nbviewer.jupyter.org/github/Akramz/Hands-on-Machine-Learning-with-Scikit-Learn-Keras-and-TensorFlow/blob/master/03.Classification.ipynb](https://www.kaggle.com/datasets/bistaumanga/usps-dataset)https://www.kaggle.com/datasets/bistaumanga/usps-dataset


