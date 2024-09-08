# How to install PtyPy

When trying to install PtyPy you might face different challenges depending on your computing environment and/or the scenario for using PtyPy. I will try to briefly go over the most common scenarios.

## Install basic PtyPy from scratch

Assuming that your operating system already has some version of Python install, it makes sense to first create a virtual environment. 
For this purpose, we can use Python's native `venv` module

```bash
python -m /path/to/venv
```

and activate it

```bash
source /path/to/venv/bin/activate
```

Next, we need to download (clone) the PtyPy source repository:

```bash
git clone https://github.com/ptycho/ptypy.git /path/to/ptypy
```

Now that we have cloned ptypy, we can use pip (which is already installed as part of the `venv`) 
to install PtyPy into our virtual environment

```bash
cd /path/to/ptypy
pip install .
```

which will install PtyPy alongside its basic dependences (numpy, scipy, h5py). 
To test that everything has been installed correctly, we can run one of the template examples:

```bash
cd /path/to/ptypy/templates
python ptypy_minimal_prep_and_run.py
```

## Install fully blown PtyPy on top of MPI and CUDA

## Install fully blown PtyPy using conda

Download the `conda` package manager from conda-forge:

```bash
wget https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Linux-x86_64.sh /path/to/installer
```