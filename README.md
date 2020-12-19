# Python Virtual Environment Summary

In this document I collect everything for a summary on Python's virtual environments.


## Why one should use virtual environments

For years I have always used the full installation of Python distributions such as WinPython oder Anaconda. This may make sense in certain settings, e.g. in the corporate world, where you can't access the outside internet world as you like due to security constraints. In a private setting however not using fully fledged distributions but virtual environments has as few advantages:

* It takes a lot less space on your disk (well, in times like these where you are likely to have more than 500 GB of space this might not be a crucial argument)
* You can define invidual environments for specific tasks, this also simplifies the deployment of individual projects
* You want to try a new package but are afraid that it might break your Python installation: test it first in a virtual environment

## Installing miniconda

I have made good experiences with the Anaconda Python distribution. Anaconda also provides Miniconda, a minimalistic Python environment that we can use to play with virtual environments. Get it from https://docs.conda.io/en/latest/miniconda.html and install it.


## Setting up your first virtual environment

```
conda create -n myenv python
```


## Configuring conda-forge

```
conda config --add channels conda-forge
conda config --set channel_priority strict 
```

## Installing packages

```
conda install 
```