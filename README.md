# Python for Marketing (pymarketing)

## Getting started

*Note for newcomers:*: We're going to use [PIP]() and [Virtualenv]() to create a separate 'sandbox' environment to install things into. Why? Well Python comes pre-installed on OSX and installing into the main environment can create clashes. You can also run multiple Virtualenv environments on the same computer, at the same time if needed.

*There are mixed opinions about which to install first. For now, it's simplest to install PIP and then Virtualenv*

### OSX instructions

1. Open up a new Terminal window
2. Type:

    `sudo easy_install pip`

3. You should be asked for your Mac's admin password.
4. After installation, type:

    `pip install virtualenv`

5. Once Virtualenv has installed you're almost ready. Head to your home directory (`cd ~/`) and create a new folder called `Code`:

    `mkdir Code`
    
    This is where you will house all of your coding files. If you'd rather rename this to something else you can, it's just a recommendation for newcomers without an existing setup.
6. Create a new subfolder in `Code` called `Virtualenv`:
    
    `cd Code`

    `mkdir Virtualenv`

    This is where you will install your first and any future Virtualenv environments.
7. Make `Virtualenv` your current directory (type: `cd ~/Code/Virtualenvs`) and you're ready to create your first Virtualenv.
8. In the Terminal, type:
	
	`virtualenv pymarketing`

	This will create a new, empty, virtualenv to install everything into in future.
9. Once that's done, you'll know it's worked because your Terminal lines will be prefixed with the name `(pymarketing)`.

    That's the generic stuff done. You can do similar for future environments - none of this is specific to Python for Marketing, except for the names we used. You're now ready to start intalling the `pymarketing` package:

    **TODO**: Add instructions on how to deactivate and reactivate the Virtualenv from the [Virtualenvwrapper page](http://virtualenvwrapper.readthedocs.org/en/latest/install.html)

10. In the same Terminal window, enter the following line to install this package from GitHub:
	
	`pip install git+https://github.com/philsheard/pymarketing.git`
11. Once the installation is complete, you will need to install all the other packages we'll be using - these are called 'dependencies' in Python. In future installs, this will happen automatically buy I need to work out how. Make sure your virtualenv is still active and then type: `pip install -r ~/Code/Virtualenv/pymarketing/lib/python2.7/site-packages/pymarketing/requirements.txt`. This will install a long list of packages we'll be using at various times. It's a lot, and some may not be used for a while, but as a newcomer this is easier than finding each one independently.
12. If that all worked, you should be able to run the following commands:
	`cd ~/Code/Virtualenv/pymarketing/lib/python2.7/site-packages/pymarketing/notebooks/`

	`ipython notebook`
13. The IPython Notebook should open in a new window on your default browser. Open the first sample notebook (`Sample_notebook.ipynb`) and we're off.