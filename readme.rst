Elevator manual
===============

Setting up a development environment
------------------------------------

To start working on website and docs, first prepare your development environment:

1.  Make sure you have Python 3.8, `make` and `poetry` installed.

    ..  code-block:: console

        $ pip install --user poetry
        $ poetry --version

        Poetry version 1.0.5

2.  Initialize a new virtual environment with `poetry`:

    ..  code-block:: console

        $ cd elevator
        $ poetry install
        $ poetry shell
        $ which python
        <shows path to your virtual environment>
        $ sphinx-build --version
        sphinx-build 3.3.1

Now your environment is ready.

Every time you open a new terminal session (window), activate the virtual environment in it:

..  code-block:: console

    $ poetry shell


Working on the website
----------------------

While you work, serve website locally with a live-reload:

..  code-block:: console

    $ make serve

This will open a browser tab with a local copy of the website.
Every time you change the sources, it will rebuild your website and refresh the browser tab.

To prepare a copy for deployment, build it in a `dirhtml` format:

..  code-block:: console

    $ make clean dirhtmlg

Publishing
----------

To publish new content, merge a pull request.
Once your code is in the `master` branch, a GitHub Action will publish it.
