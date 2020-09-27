<html>
<h3>Convolutional neural network for stock price prediction using transfer learning</h3>
This repository contains the python code for the research paper "Convolutional neural network for stock price prediction using transfer learning", which is based on the WorldQuant University capstone project by the author.

<br>
<br>
<h3> Envorinment and Installation</h3>
Python code are stored in the code directory in a jupyter notebook format. The notebooks run on <a href="https://colab.research.google.com/notebooks/intro.ipynb">google colab</a>, 
but they may not work in a local environment. The latest tensorflow version for the Convolutional Neural Network (CNN), which only works within the google colab environment is used.   
Google drive is used to store the training and test images data. In order to access to the google drive from the google colab, you need to mount on google drive from the google colab. 
Packages required for the execution of the code are installed at the begining of the jupyter notebooks. You also need to create directories in advance. 
You need a directory for training data and another directory to store the test data. In each directory, you need to create three sub directories labeled as up, flat, or down.

<br>
<br>
<h3> Jupyter Files </h3>
Candle_stick2.ipynb is a file for downloading the data and creating candle sticks images. After creating candle stick images, the code automatically label the date, assign a unique file name, 
and store them into the appropriate directories.
<br><br>
Candle_CNN.ipynb is a file for the CNN model. The candle stick images which are created by the Candle_stick2.ipynb and stored in the training directory are fed into the CNN model. 
We use a pretrained CNN model <a href="https://github.com/tensorflow/models/tree/master/research/inception">Inception v3</a>, which is created by google. It is pretrained on Imagenet images. We add three additional layers at the end of the inception V3 and execute the training of the model for the additional layers. The parameters of the original inception v3 layers are not changed.
The model are evaluated on the test set alongside the training.

<br>
<hr>
<h3>Contact</h3>

Yohei Komori <br>
Email: hurumori@gmail.com
</html>