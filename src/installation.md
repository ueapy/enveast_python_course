![](danger.jpg)

# Installation instructions

For this workshop we will be running Python in IT labs at UEA. However, if you want to run Python on your own PC, follow the instructions below to set up your environment. The only requirement is that you have to do this **before** the course! Feel free to contact [Denis](mailto:d.sergeev@uea.ac.uk) if you have any problems with the installation (but better google them first!)

Note: **the course is designed in Python 3.5**

## Local PC

The best way to set up Python for this course is with [conda](http://conda.pydata.org/docs/).

1. Install [Anaconda](https://www.continuum.io/downloads) or, its lighter version, [Miniconda](http://conda.pydata.org/miniconda.html). Use Python 3.5 version! [Determine if your OS is 32-bit or 64-bit](http://www.computerhope.com/issues/ch001121.htm)

2. Once Anaconda/Miniconda distribution is installed, open a command line (Terminal.app on OSX or cmd.exe on Windows) and run the following instructions.

### Unix / OSX
```
git clone https://github.com/ueapy/enveast_python_course_materials.git
```
```
cd enveast_python_course_materials
```
```
conda env create -f environment.yml
```
This should create a new conda environment named "course2016".

If your default shell is NOT bash, first type `bash`. To activate or switch to your new conda environment, you should *activate* it from a command line:
```
source activate course2016
```
Note that a prefix should appear in the command line.

To switch and/or deactivate environments:
```
source deactivate
```

### Windows
* Download the configuration file named [`environment.yml`](https://github.com/ueapy/enveast_python_course_materials/blob/master/environment.yml).
* In the command line, check that the file is in the current directory and then type
```
conda env create -f environment.yml
```
To activate or switch to your new conda environment, you should *activate* it from a command line:
```
activate course2016
```
Note that a prefix should appear in the command line.

To switch and/or deactivate environments:
```
deactivate
```

## Cloud service
It is also possible to run this course using a temporary session on [binder](mybinder.org).
