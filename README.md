# cgca-ml-tutorial
This is an introductory python based machine learning (ML) tutorial
using the [scikit-learn](http://scikit-learn.org/stable/) library. The application is mostly
centered in areas of physics and astronomy.

## Getting started
The code is mostly in Python. However, to get the codes and the data,
one must have `git` installed. On Ubuntu/Debian systems, this can be done using
```bash
sudo apt-get update
sudo apt-get install git
```

Additionally, the codes are in Python >= 3.5. Since most system installations
are Python 2.7.x, we have to work in a virtual environment. This is done
using `virtualenv`, which can be installed (in Ubuntu/Debian systems) using:
```bash
sudo apt-get install virtualenv
```

It is a good practice to have a directory (say `virtualenvs` under your home
directory) to store all virtual environments you create. Let's create a
`python 3` environment under it and activate it.
```bash
mkdir ~/virtualenvs
cd ~/virtualenvs
virtualenv cgca-ml-tuto --python=python3
source cgca-ml-tuto/bin/activate
```

In case of other systems (or even Unix systems), using [Miniconda](https://conda.io/docs/user-guide/install/)
is a robust way to create virtual environments. Ensure to use the `python3` installer. Once installed
the instructions to create and activate a virtual environment can be found [here](https://conda.io/docs/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands).

At this point the name of the virtual environment should be prepended to your
command prompt as:
```bash
(cgca-ml-tuto) user@localhost:~/virtualenvs$
```

Navigate to a location where you would like to clone a copy of this repository.
As a good practice, one could have a directory named `github` under the home
directory and then clone this and future repositories. Run the following to clone
this repository:
```bash
git clone https://github.com/deepchatterjeeligo/cgca-ml-tutorial.git
```
This should create a directory named `cgca-ml-tutorial` containing the required
notebooks and data.

You are ready to install the required libraries using `pip`. Double check that
you have the correct `pip` in you `PATH` by running
```bash
which pip
```
This should point to the `pip` under the `bin` directory of the virtual environment
you just created, namely `cgca-ml-tuto` in this case.

Now install all dependencies. Here, I list out all of them to be install with `pip`:
```bash
pip install numpy scipy astropy pandas seaborn matplotlib scikit-learn jupyter
```

If successful, you have a working virtual environment, separete from you system
installation, with all the libraries needed for this tutorial!
`jupyter` is not necessary to run the codes, but to see and run the notebooks.
