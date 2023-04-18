# Lecture 102: Introduction to Anaconda

This course focuses on python, we will use python3 as python2 is not supported anymore.

Similarly, we will use jupyter notebooks (.ipynb) for the courses taught in this class.

The extension .ipynb stands for interactive python notebooks.

- Jupyter notebooks are useful tools for learning programming because they provide a visual interface.

- You can see the results of your code live, instead of waiting till your script (.py) finishes running in a terminal.


To be able to use python and jupyter notebooks in your laptop/PC, there are several options:

# 1. Google Colab (see https://colab.research.google.com/):
One option is to use Google Colab, which we will use in the classroom. For this you would need a Gmail account, which is conveniently provided by Yachay Tech.

- The advantage of using Google Colab is that all libraries are installed in a Linux server remotely, so we don't need to worry about compatibility issues, different operating systems, etc.
- The disadvantage is that Colab provides limited memory resources and very limited disc space since everything is stored in a cloud, so you can only use it to process small datasets.

## How do I test Google Colab?
1. Download this notebook: [https://github.com/wbandabarragan/computational-physics-1/blob/main/unit-1/101-Introduction-GoogleColab.ipynb](https://github.com/wbandabarragan/computational-physics-1/blob/main/unit-1/101-Introduction-GoogleColab.ipynb)
2. Open Goole Colab (you will need to log into your Yachay email accounts).
3. Upload the notebook, and run it. If you see the plots, Google Colab works.

# 2. Anaconda/Miniconda (Recommended, see https://anaconda.org/):
Another option is to have python (and all the libraries you need to analyse your datasets) installed in your laptop/PC. This can also be done in many ways, but anaconda is now very popular because it provides good portability and an interface that allows the user to include extra kernels for other programming languages. Anaconda has the advantage that you have all the code you need locally in your laptop. In the long term, using Anaconda will be much more advantageous.

# Installation instructions

## How to install Anaconda?
Download Anaconda from this website: https://www.anaconda.com/products/individual. Choose the package version that best suits the operating system (OS) of your laptop.

### On Linux and MacOSX:
For testing and customising your installation on Linux/MaxOSX laptops/PCs, follow these instructions:

#### Installation from a terminal (recommended)

1. Open a terminal window.<br>

2. Type the command below:<br>
~~~~html
  $ conda --version
  conda 4.10.3
~~~~

3. That means you have Anaconda 4.10.3 installed.<br>

4. Now, let us check which environment you have:<br>
~~~~html
  $ conda env list
  conda environments:
  base                  *  /Users/webb/opt/anaconda3
~~~~

5. Let us know create a new environment with:<br>
~~~~html
  $ conda create -n py37 python=3.7
  $ conda env list
  conda environments:
  base                  *  /Users/webb/opt/anaconda3
  py37                     /Users/webb/opt/anaconda3/envs/py37
~~~~

6. Now, we activate the environment:<br>
~~~~html
  $ conda activate py37
  $ conda env list
  conda environments:
  base                     /Users/webb/opt/anaconda3
  py37                  *  /Users/webb/opt/anaconda3/envs/py37
~~~~

7. Let us check with libraries are installed by default:<br>
~~~~html
  $ conda list
~~~~

8. Let's install a few extra libraries:<br>
~~~~html
  $ conda install jupyter numpy cython mpi4py git
~~~~

9. Type 'yes' to accept changes, and check that the new libraries are present.<br>
~~~~html
  $ conda list
~~~~

10. Let's now open a jupyter notebook, and we are ready to work.<br>
~~~~html
  $ jupyter notebook
~~~~

10. Once the notebook is open, you can start coding your first notebook:<br>

[https://github.com/wbandabarragan/computational-physics-1/blob/main/unit-1/101-Introduction-GoogleColab.ipynb](https://github.com/wbandabarragan/computational-physics-1/blob/main/unit-1/101-Introduction-GoogleColab.ipynb)


### On Windows:
If you are using Windows, I highly recommend either:

1. setting up a dual partition in your hard drive with both Windows and Linux (make sure you back up your data before), or
2. setting up a Virtual Machine (VM) with a linux distribution. For this:

- Download VirtualBox from: https://www.virtualbox.org/
- Follow the instructions here: https://itsfoss.com/install-linux-in-virtualbox/

After the installation of the VM is successful, follow the instructions provided above for Linux/MacOSX systems to set up your Anaconda installation.

In the long term, you may want to fully switch to Unix-based operating systems. Ubuntu is a popular and user-friendly option:

Ubuntu webpage: https://ubuntu.com/


## How do I test and use Anaconda?
Assuming all the steps above went well, and you were able to create your first jupyter notebook, open a new notebook and follow these two tutorials on jupyter notebooks and basic python:

- https://datacarpentry.org/python-ecology-lesson/jupyter_notebooks/
- https://swcarpentry.github.io/python-novice-gapminder/

Please make sure you are familiar with the material above as there will be little time to cover technicalities.
