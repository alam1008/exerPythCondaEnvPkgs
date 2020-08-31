# Setting up Environments and Installing Packages Using Conda

## Summary of steps to complete

- [ ] Fork this repository so you have your own copy to work on.
- [ ] Clone the repository on your local machine. 
- [ ] Edit this README.md file on your machine.
- [ ] Run the Conda commands shown in the video and describe them in the table below.
- [ ] Push your changes to your GitHub repository.
- [ ] Submit a link to this GitHub repository in Canvas.

## 1. Fork & Clone this repository

* We did this in a previous assignment. Instructions are here: https://github.com/cmcntsh/N6806_Fall2020_DevNotes/blob/master/Projects/002%20-%20Practice%20Using%20Git%20and%20GitHub/README.md
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

## Conda Concepts

* [ ] Describe the Conda concepts used in the video and listed in the table below.

|   Concept   |         Description or short answer         |
|     ---     |                     ---                     |
|What is the purpose of having different environments?     |(Virtual environments allow for the creation of Python projects serving different purposes (i.e. web development, data analysis, artificial intelligence/machine learning). This is helpful for running multiple projects with different Python applications requiring different version specifications and packages.)|
|What is the default package manager in Python?            |(Pip)|
|How do you manage environments and packages in Anaconda?  |(Conda is a package that comes with Anaconda. It allows you to manage packages and virtual environments.)|
|`conda list`       |(A list that shows all the default packages that were installed when Anaconda was installed.)|
|`conda env list`       |(A list that shows all the default environments installed.)|
|How do you keep your base environment unchanged?       |(You can keep your base environment unchanged by creating different virtual environments using the command 'conda create --name XXXX')|
|What is the link to the Conda cheat sheet? (link in video notes is broken)      |(https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf)|
|`conda create --name XXXX`    |(Create a new environment and download/extract packages.)|
|`source activate XXXX`       |(To activate new environments.)|
|`conda install YYYY`       |(To download packages to current environment.)|
|channels in Conda       |(The location where packages are stored. Conda will search for packages in default channels.)|
|`conda install -c ZZZZ YYYY`       |(To install packages from a specific channel. This is only a one-time installation.)|
|`conda config --show channels`       |(To show the channels available in Conda.)|
|`conda config --add channels ZZZZ`       |(To add specific channels to the default list in Conda.|
|conda-forge.org       |(Community-led collection of Python packages. Here you can access conda-forge specific packages, which are only available through this channel.)|
|`source deactivate`       |(To deactivate an active environment.)|
|`conda config --get channels`       |(View list of channels and their priority. Conda will check for packages in channels with the highest priority first. This can be helpful when you have different versions of certain packages in different default channels.)|

* After creating the environments he created in the video on your computer, what would the results of running the command `conda env list` look like with the da35 environment activated. Paste the output from your command prompt in the code block below.

```
base                     /opt/anaconda3
ai37                     /opt/anaconda3/envs/ai37
da35                  *  /opt/anaconda3/envs/da35

```
* What command would you use to remove the environments you created for this exercise from your computer?

```
conda env remove --name ai37
conda env remove --name da35

```
