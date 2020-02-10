# Intro-to-Data-Engineer Installation
## 1 Install the Python development environment on your system
Open terminal via Ctrl+Alt+T or searching for “Terminal” from app launcher.
```shell
sudo apt update # update apt
sudo apt install python3-dev python3-pip # install python 3 and pip
sudo pip3 install -U virtualenv  # system-wide install
```
## 2 Create a virtual environment
Create a new virtual environment by choosing a Python interpreter and making a ./venv directory to hold it:
```shell
virtualenv --system-site-packages -p python3 ./venv 
```
*** the venv will create at the current directory ***
Activate the virtual environment using a shell-specific command:
```shell
source ./venv/bin/activate  # sh, bash, ksh, or zsh 
```
When virtualenv is active, your shell prompt is prefixed with (venv).
Install packages within a virtual environment without affecting the host system setup. Start by upgrading pip:
```shell
pip install --upgrade pip

pip list  # show packages installed within the virtual environment
```
And to exit virtualenv later:
```shell
deactivate  # don't exit until you're done using TensorFlow
```

## 3 Install python library to your virtual environment
```shell
pip install mysql-connector
pip install apache-airflow
```
