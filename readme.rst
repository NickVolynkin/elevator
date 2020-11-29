Elevator manual
===============

Collaboration
-------------

To start working on website and docs, first prepare your development environment:

1. Make sure you have Python 3.8 and `poetry` installed.

..  code-block:: console

    $ pip install poetry
    $ poetry --version

    Poetry version 1.0.5

2. Initialize a new virtual environment with `poetry`:

..  code-block:: console

    $ cd elevator
    $ poetry install
    $ poetry shell
    $ sphinx-build --version

    sphinx-build 3.3.1

3. Now build a project:

..  code-block:: console

    $ make dirhtml

4. Open ./build/dirhtml/index.html with your browser.

