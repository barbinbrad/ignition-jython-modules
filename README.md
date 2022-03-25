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
