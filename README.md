# OpenCV-3.1-Mac-Python-Installer
Install OpenCV 3.1 and Python 3.5 on Mac OS X , including modules


## Install Conda

```shell

# Download the latest Conda edition for a 64-bit machine (this assumes you are running python 3.5)
cd ~/Downloads
wget https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh

# Move conda to an Installation directory
mkdir ~/Installations && cd Installations
mv ~/Downloads/Miniconda3-latest-MacOSX-x86_64.sh .

# Install Miniconda
bash Miniconda3-latest-MacOSX-x86_64.sh

# Follow instrunctions at the terminal prompt
# Accept license agreements
# Allow for environment variables
# Set the Conda installation destination to your ~/Installations/Miniconda3 directory
```

Close and reopen the terminal for changes to take affect

Test the installation with `conda list`


# Install Python 3.5.x

```shell
conda install numpy
...
$ conda create -n py3k anaconda python=3
...

# Update conda
conda update conda
```


# Install the OpenCV 3.1.x package via Conda

```shell
conda install -c menpo opencv3=3.1.0
```


# Test the installation
```shell
python3
>>> import cv2
>>> cv2.__version__
'3.0.0'
```


# opencv/opencv_contrib Modules installation
OpenCV modules are now contained in the opencv_contrib modules repository

## Instll XCode
[https://developer.apple.com/xcode/]()


## Download the opencv_contrib modules
```
cd ~/Installations
wget https://github.com/opencv/opencv_contrib/archive/master.zip
unzip master.zip

# Rename the directory 
mv opencv_contrib-master opencv_contrib
```

## Download the CMake .dmg from the CMake website
```shell
cd ~/Installations
wget https://cmake.org/files/v3.7/cmake-3.7.0-Darwin-x86_64.dmg
```





