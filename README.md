# Finetuning-Hyperparameters-in-Deep Neural Network
This project is based on the Digit Recognizer competition on Kaggle, found here: https://www.kaggle.com/c/digit-recognizer/data.
To sum it up in a nutshell, it is about predicting the correct handwritten digit based on its image pixels. The dataset is the famous MNIST-dataset by Yann LeCun at al. (http://yann.lecun.com/exdb/mnist/). 
<br>
<br>
There are several ways to solve this "problem" (for example with a K-Nearest-Neighbor algorithm, found in my repository here: https://github.com/IIIskiplikIII/another-MNIST-try). 
<b>This time instead I chose the Deep Neural Network approach.<b>

## Installing
You need Jupyter Notebook to start and execute this notebook. A good way to install it is with Anaconda. 
There are as well other ways to use it, for example by uploading it in a Google Colab. 
For that, you need to download/upload the data folder into your Google Colab.

### Requirements / Environemnt
There is an environment.yml (conda) file to create your conda environment with all the necessary dependencies. The following dependencies are used:
  - numpy
  - pandas
  - scikit-learn
  - matplotlib
  - tensorflow=2.3.0

### Base Path
If you want to run this notebook on your local machine you need to configure the base path in the first cell of the notebook (were alls the imports are made):

```python
# change your local path here
if kaggle == 1 :
    MNIST_PATH= '../input/digit-recognizer'
else:
    MNIST_PATH= '../Digit_Recognition_with_a_Deep_Neural_Network/data/input/digit-recognizer'
```

As you can see there is a switch to change the base path if you want to run it on Kaggle or local. 1 = Kaggle / 0 = local.

### Tensorboard
By installing Tensorflow, the tensorboard should be installed as well.
