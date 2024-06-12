Installing useful python packages
===============================================================================

Before doing anything, make sure:

- anaconda is up-to-date as well as installed packages.
- you are using a decent version of python (ideally the latest stable version).

To do so, you might want to run the following commands:

```bash
# Update anaconda
conda update -n base -c defaults conda
# Update all packages
conda update --all
# List the versions of Python that are available to install
conda search python
# Create a "tuto" environment with the latest available version
# of python (here 3.10)
conda create -n tuto python=3.10 anaconda
```

## Libraries to install with anaconda

```bash
 # Go there first to install pytorch with the command line
 # that corresponds to your system:
 # https://pytorch.org/get-started/locally/
 conda install pytorch torchvision torchaudio pytorch-cuda=11.6 -c pytorch -c nvidia
 conda install -c pytorch torchtext
 conda install -c anaconda numpy
 conda install -c anaconda scipy
 conda install -c anaconda scikit-learn
 conda install -c anaconda pandas
 conda install -c anaconda pillow
 conda install -c anaconda jupyter
```

## Libraries that are standard python libraries (so no need to worry)

- collections
- datetime
- math
- os
- sys
- typing