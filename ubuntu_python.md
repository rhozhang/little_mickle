# ubuntu and python

Ubuntu uses python for many system related functionalities. You must not remove the Python installation that is 
preinstalled by it, or you'll end up with a broken system

If for some reason you need to use a more recent Python version, just install it parallel and call it explicitely, 
e. g. with python3.9, as python3 will point to the default installation (python 3.8.5 for ubuntu 20.04). 
The same goes for pip, which may need the --user option or being called with sudo depending on the permissions

**THINK AHEAD BEFORE REMOVing PYTHON FROM UBUNTU!**

but if you have removed the python, you will fail to start ubuntu by gui mode. How to restore?

Ctrl + Alt + F2 to enter terminal

```bash
sudo apt install ubuntu-minimal \
                 ubuntu-standard \
                 ubuntu-desktop
```

reboot, and you can use gui again

