Herschel Extragalactic Legacy Project python module
===================================================

This Python module aims at facilitating the work with HELP data. It also
contains tools that are useful while building the project database.

Installation
------------

While we are developing HELP, it's better to install the package in development
mode. Provided you installed [Anaconda](https://www.continuum.io/) or
[miniconda](http://conda.pydata.org/miniconda.html) here are the commands to
run (from within the cloned GitHub repository):

```Shell
$ conda create -n herschelhelp python=3
$ source activate herschelhelp
$ pip3 install -e herschelhelp/.
$ python herschelhelp/database_builder/__init__.py
```

You will need to activate this new environment with `source activate
herschelhelp` when you want to use this module or its command.

Command line
------------

This module provides a `herschelhelp` command line for an easy access to some
tools. This command has (will have) several sub-commands to perform various
tasks. Running the command alone will show the list of available (sub)commands.
Running `herschelhelp <COMMAND> --help` will display the help on the given
command.

*Note for macOS users: to be able to use the command line, the locale of the
system must be set to an UTF-8 one, see [this
page](http://click.pocoo.org/5/python3/#python3-surrogates).*

Running inside a Jupyter notebook
---------------------------------

If one need to use this code inside a Jupyter notebook, one should install the
notebook stuff:

```Shell
$ conda install notebook
```

and add the environment Python to the list of kernels for Jupyter:

```Shell
$ python -m ipykernel install --user --name helpext --display-name "Python (herschelhelp_python)"
```

The notebooks must be set to use this kernel.

*Note: maybe it's not mandatory to install the full notebook and only the
ipykernel is required if Jupyter is already installed on the system.*
