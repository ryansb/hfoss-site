hfoss-site (content repository)
===============================

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
