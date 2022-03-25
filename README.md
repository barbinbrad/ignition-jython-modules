## What is this?

This is a collection of pre-built jython modules that can be added to Ignition to support easy import of the following libraries:

1. [requests](https://docs.python-requests.org/en/latest/)
2. [bottle](https://github.com/bottlepy/bottle#bottle-python-web-framework)
3. [paho.mqtt](https://github.com/eclipse/paho.mqtt.python#usage-and-api)
4. [sparkblug_b](https://github.com/eclipse/tahu/blob/master/sparkplug_b/stand_alone_examples/python/example_simple.py) 

## Install modules for Ignition
```
git clone https://github.com/barbinbrad/ignition-jython-modules
rsync -r --exclude '.git' ignition-jython-modules/. /usr/local/ignition/user-lib/pylib
```

## Add modules to Repo

1. Install jython
2. Clone the repo of the module to be installed
3. Run `jython install setup.py` in the cloned repo
4. Copy the results from `jython/Lib/site-packages` to this repo
5. Open an MR
6. Close Ignition and run the scripts above
