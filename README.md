# jupyterlab_commands
Support for arbitrary python commands

[![Build Status](https://travis-ci.org/timkpaine/jupyterlab_commands.svg?branch=master)](https://travis-ci.org/timkpaine/jupyterlab_commands)
[![PyPI](https://img.shields.io/pypi/l/jupyterlab_commands.svg)](https://pypi.python.org/pypi/jupyterlab_commands)
[![PyPI](https://img.shields.io/pypi/v/jupyterlab_commands.svg)](https://pypi.python.org/pypi/jupyterlab_commands)
[![npm](https://img.shields.io/npm/v/jupyterlab_commands.svg)](https://www.npmjs.com/package/jupyterlab_commands)



## About
This code lets you inject arbitrary commands into the JLab frontend:
![](https://raw.githubusercontent.com/timkpaine/jupyterlab_commands/master/docs/4.gif)
![](https://raw.githubusercontent.com/timkpaine/jupyterlab_commands/master/docs/1.png)
![](https://raw.githubusercontent.com/timkpaine/jupyterlab_commands/master/docs/2.png)
![](https://raw.githubusercontent.com/timkpaine/jupyterlab_commands/master/docs/3.png)


## Install
```bash
pip install jupyterlab_commands
jupyter labextension install jupyterlab_commands
jupyter serverextension enable --py jupyterlab_commands
```

## Adding commands
install the server extension, and add the following to `jupyter_notebook_config.py`

```python3
c.JupyterLabCommands.commands = {'command display name', python_function, ...}
```