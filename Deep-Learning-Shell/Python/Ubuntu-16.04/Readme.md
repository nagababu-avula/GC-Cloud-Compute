### Ubuntu 16.04 Shell Installation
#### Organization:      George Washington University 

### All the below deep learning frame works are installed in python

#### Torch with Lua Caffe in Python 2.7, Caffe2 in Python 2.7, Tensorflow in Python 2.7 and 3.5, 
#### Theano in Python 2.7 and 3.5, Pytorch in Python 2.7 and 3.5.

##### * To activate the virtual python, check the testing software installation section.
##### * Before Installing Check whether enough storage space available (minimum 30GB) 
##### * and good to have minimum 2 CPUs with 8GB RAM

```
sudo apt-get install git -y
git clone https://github.com/nagababu-avula/GC-Cloud-Compute.git
cd GC-Cloud-Compute/Deep-Learning-Shell/Python/Ubuntu-16.04/

mv install-16-04.sh ~
cd ~
chmod +x install-16-04.sh
sudo ./install-16-04.sh <username of ssh key>
```

## Testing the framworks
### Torch

Run the following commands

```
source /etc/environment
source ~/.bashrc
```
then to test torch just enter
```
sudo ~/torch/install/bin/luarocks install torch 
th
```
in to your terminal and you should be able to see the torch environment. Now enter ``` require 'dp' ```
if torch is is installed correctly then you should be see a long list. 

If the GPU is intsalled correctly then after entering the following command you sould see the true output.
```require 'cunn'```

Then type ```exit``` and then enter ```'y'``` to get out of the torch env.

### Caffe
Enter the following command on your terminal
```
python
```
then in the python env write ```import caffe```
exit out from python env by ```exit()```

### Caffe2 - Version 2
Enter the following command on your terminal
```
python
```
then in the python env write ```import caffe2```
exit out from python env by ```exit()```

### Tensorflow, Keras, Theano (python 2.7)
Enter the following command on your terminal
```
source ~/python2/bin/activate
python
```

then in the python env write
```
import tensorflow
import keras
import theano
```

if you did not get any error then exit out from python env by 
```exit()```.

Enter the following command to get out of the virtualenv. ```deactivate```.

### Pytorch (python 2.7)
Enter the following command on your terminal
```
python
```
then in the python env write
```
import torch
import torchvision
```
if you did not get any error then exit out from python env by 
```exit()```.

### Tensorflow, Keras, Theano (python 3.5)
Enter the following command on your terminal
```
source ~/python3/bin/activate
sudo pip3 install pandas --upgrade
sudo pip3 install --upgrade numexpr
python3
```

then in the python env write
```
import tensorflow
import keras
import theano
```

if you did not get any error then exit out from python env by 
```exit()```.

Enter the following command to get out of the virtualenv. ```deactivate```.

### Pytorch (python 3.5)
Enter the following command on your terminal
```
python3
```
then in the python env write
```
import torch
import torchvision
```
if you did not get any error then exit out from python env by 
```exit()```.

### Pycharm and ZeroBraneStudio

* Note: Mac users need to acivate [Xquartz](https://www.xquartz.org/) in their machine and then open your terminal. In other words, when you are ssh ing to VM use -X as follows:

```
ssh -X -i <private key file > <netid>@<External Ip address>
``` 
Note: Windows users use Mobaexterma and you are fine.

To activate pycharm enter the following commands 
```
pycharm-community
```
To activate ZeroBraneStudio
```
zbstudio
```

