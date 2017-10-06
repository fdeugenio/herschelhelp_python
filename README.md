Herschel Extragalactic Legacy Project python module
===================================================

This Python module aims at facilitating the work with HELP data. It also
contains tools that are useful while building the project database.

Installation
------------

While we are developing HELP, it's better to install the package in development
mode. Provided you installed [Anaconda](https://www.continuum.io/) or
[miniconda](http://conda.pydata.org/miniconda.html) here are the commands to
run:

```Shell
$ conda create -n herschelhelp python=3
$ source activate herschelhelp
$ conda install astropy click sqlalchemy scipy
$ pip install -r requirements.txt
$ python setup.py develop
$ python database_builder/__init__.py
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
