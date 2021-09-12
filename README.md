# Setting up Environments and Installing Packages Using Conda

## Summary of steps to complete

- [ ] Fork this repository so you have your own copy to work on.
- [ ] Clone the repository on your local machine. 
- [ ] Edit this README.md file on your machine.
- [ ] Run the Conda commands shown in the video and describe them in the table below.
- [ ] Push your changes to your GitHub repository.
- [ ] Submit a link to this GitHub repository in Canvas.

## 1. Fork & Clone this repository

* We did this in a previous assignment. Instructions are here: https://github.com/cmcntsh/exerGitPractice
* This can also be done directly in VSCode
  * Create a new folder on your machine where you want to put this repository if you don't already have one you want to use.
  * Copy the Clone or Download path for this repository from GitHub.
  * In VSCode from the command pallette (Ctrl-Shift-P) run Git: Clone
  * Paste the path into the path field which pops up
  * Select your new folder you created on your machine
  * A new folder for the repository with the repository files should be in the folder you selected showing in the Explorer window in VSCode on the left side.
  
## Edit your README.md file

* [ ] In an editor of your choice (i.e. VSCode) edit this README.md file to add the answers requested in the tables.

## Follow along with this tutorial

* Conda What and Why? (27 min): https://www.youtube.com/watch?v=23aQdrS58e0&list=PLG9A6ovzPqX6d9uWzx0UYN9pm0zzl5ofA&index=13&t=0s
  * He installs Miniconda. We will be using Anaconda. Don't install Miniconda.
  * Follow along with the rest of the tutorial.
  * Go ahead and create the environments as he creates them in the tutorial.
  * (2021 update: I recommend managing environments as shown in the new Anaconda introduction video. https://anaconda.cloud/tutorials/getting-started-with-anaconda-individual-edition%3Fsource%3Dindividual-edition-tutorial) If you want to try creating the environments using the user interface for Anaconda Navigator instead of the command line shown in the Conda What and Why tutorial, that's fine. But watch the Conda What and Why tutorial to understand some of the differences between Conda environments and other types of virtual environments available in Python.

## Conda Concepts

* [ ] Describe the Conda concepts used in the video and listed in the table below.

|   Concept   |         Description or short answer         |
|     ---     |                     ---                     |
|What is the purpose of having different environments?     |(They all do different things, for example, web development, data analysis or AI.  It allows for multiple projects in one one computer.)|
|What is the default package manager in Python?            |(PIP)|
|How do you manage environments and packages in Anaconda?  |(Create a new environment, activate it and then add the needed packages to the environment)|
|`conda list`       |(Shows all the packages that are included when Anaconda was installed.)|
|`conda env list`       |(It lists the environments)|
|How do you keep your base environment unchanged?       |(Install the packages separately and only have them accessible via what you want to be your base environment.)|
|What is the link to the Conda cheat sheet? (link in video notes is broken)      |(N/A)|
|`conda create --name XXXX`       |(Creates a new environment)|
|`source activate XXXX`       |(Activates the environment)|
|`conda install YYYY`       |(Where Conda looks for the packages that need to be installed.)|
|channels in Conda       |(enter description or short answer here)|
|`conda install -c ZZZZ YYYY`       |(Allows a specific channel to be used for installation)|
|`conda config --show channels`       |(Shows if the package is availble to be entered through a specific path)|
|`conda config --add channels ZZZZ`       |(Allows for a channel to be used everytime for a package)|
|conda-forge.org       |(Site that contains additional packages that can be installed)|
|`source deactivate`       |(Takes you back to your base channel)|
|`conda config --get channels`       |(Looks at the priority of which channel Anaconda will search for first)|

* After creating the environments he created in the video on your computer, what would the results of running the command `conda env list` look like with the da35 environment activated. Paste the output from your command prompt in the code block below.

```
#Paste your results here.
# packages in environment at C:\Users\ricke\anaconda3\envs\da35:
#
# Name                    Version                   Build  Channel
blas                      1.0                         mkl
ca-certificates           2021.7.5             haa95532_1
certifi                   2021.5.30        py38haa95532_0
intel-openmp              2021.3.0          haa95532_3372
mkl                       2021.3.0           haa95532_524
mkl-service               2.4.0            py38h2bbff1b_0
mkl_fft                   1.3.0            py38h277e83a_2
mkl_random                1.2.2            py38hf11a4ad_0
numpy                     1.20.3           py38ha4e8547_0
numpy-base                1.20.3           py38hc2deb75_0
openssl                   1.1.1l               h2bbff1b_0
pip                       21.0.1           py38haa95532_0
python                    3.8.11               h6244533_1
setuptools                52.0.0           py38haa95532_0
six                       1.16.0             pyhd3eb1b0_0
sqlite                    3.36.0               h2bbff1b_0
vc                        14.2                 h21ff451_1
vs2015_runtime            14.27.29016          h5e58377_2
wheel                     0.37.0             pyhd3eb1b0_1
wincertstore              0.2                      py38_0

```
* What command would you use to remove the environments you created for this exercise from your computer?

```
#Type the command here. 
conda env remove --name *** Or delete it from Anaconda Navigator

```
## 2021 Update
Python, Anaconda, and many programming languages are constantly evolving. The video Conda What and Why provides a great explanation of why you may want to use virtual environments for your Python projects, and it provides a nice demonstration of how to work in the command line. However, environment management using Anaconda Navigator is more user friently than ever. I personally will be using Anaconda Navigator to manage environments and packages since it seems easier to see what is going on using the GUI. If you haven't done so already watch the introduction to Anaconda video and pay close attention to the section on using Anaconda Navigator to create environments and install packages. https://anaconda.cloud/tutorials/getting-started-with-anaconda-individual-edition%3Fsource%3Dindividual-edition-tutorial
