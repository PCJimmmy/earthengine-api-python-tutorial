Tutorial to get started with Google's Earth Engine API in Python.

# Installation

You will have to resolve some minor issues on your own while setting up the environment.
I've mentioned the errors I encountered and how to tackle them:

- pip install earthengine-api (will automatically install google-api-python-client as well)
- Check for installations of (openssl and pyopenssl) or (pycrypto). pyCrypto is recommended as per documentation.
- pip install oauth2client
- Try importing 'ee' module in python. If it shows the error- ImportError: cannot import name 'opentype'
You need to upgrade the pyasn1 module.
- Uninstalling/Reinstalling pyasn1 will give an error saying it is a disutils installed project and would uninstall partially. Use blockstage command:
pip install --ignore-installed pyasn1
This should install the latest version 0.4.4 and you should be good to go!

## Setting up Earth Engine

- Request permission: https://signup.earthengine.google.com (Max 2-3 days)
- Login via gmail account to https://code.earthengine.google.com
- Generate the authentication token as described in the notebook (authentication.ipynb)
