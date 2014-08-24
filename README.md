hfoss-site (content repository)
===============================

# Setting up Your Enviornment

Before you can do anything with this
(run the webserver locally, or any of the
scripts) you'll need to setup and activate
a python [virtualenv](http://pypi.python.org/pypi/virtualenv).
And then run the following commands at the prompt.

## On Linux/Mac OS X

If you don't have virtualenv installed yet, try:
```
sudo easy_install virtualenv virtualenvwrapper
```

If you're using a distro like Fedora or Ubuntu,
you should try this instead:

Fedora:
```
sudo yum install python-virtualenv
```

Ubuntu:
```
sudo apt-get install python-virtualenv
```

Once you have virtualenv installed, you
should be able to run
```
cd code
git clone git@github.com:YOUR_USERNAME/hfoss-site.git
virtualenv --no-site-packages -p python2 hflosskenv
. hflosskenv/bin/activate
cd hflossk
python setup.py develop
```

## On Windows

At the windows command prompt:
```
virtualenv --no-site-packages -p python2 hflosskenv
hflosskenv/Scripts/activate.bat
```

In msysGit or git-bash:
```
git clone git@github.com:YOUR_USERNAME/hfoss-site.git
```

Back in the windows command prompt:
```
cd hflossk
python setup.py develop
```

# Testing Your Changes

To be careful, you should run the server locally
(on your machine) to check that whatever
modifications you made to the files actually renders
the way you want.

In order to do that, first make sure you have your 
virtualenv activated. And the hflossk pip module installed.

To install the hflossk pip module simply run:
```
sudo easy_install hflossk
```

Being certain of that, in the root directory, simply run:
```
hflossk run
```

You *should* see a success message such as

> Running on https://127.0.0.1:5000/
> Restarting with reloader

Open that URL in your browser to view the site
