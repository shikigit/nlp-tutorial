Tutorial: Natural Language Processing in Python
=====

This repo contains material for a workshop on Natural Language Processing with Python.

Environment Set up
-----

The code has been tested with Python `3.4` and `3.5`. This paragraph describes how to set up your environment locally.

Step 1 - clone this repo::

    git clone https://github.com/bonzanini/nlp-tutorial
    cd nlp-tutorial

Step 2 - create and activate a Python virtual environment::

    virtualenv nlp-venv
    source nlp-venv/bin/activate

Step 2 (alternative) - create a Conda environment::

    conda create --name nlp-venv python=3.5
    source activate nlp-venv

Step 3 - install libraries::

    pip install -r requirements.txt

This will download and install NLTK, scikit-learn and jupyter (plus dependencies).

NLTK requires some data to be installed separately (more details on `the NLTK website <http://www.nltk.org/data.html>`_).

From the command line, you can download the required packages::

    python -m nltk.downloader punkt stopwords reuters

Alternatively, from a Python interactive shell::

    >>> import nltk
    >>> nltk.download()

Then use the GUI to select the requires packages (punkt, stopwords, reuters).

Tip: even if you can use "all" as package name to install all the NLTK data, it's not a great thing to do over a flakey conference wi-fi. This will download approx. 2Gb and if we all do it at the same time we'll kill the conference wi-fi :)

Finally - run Jupyter::

    jupyter notebook


Authors
-----

Main authors:

- Marco Bonzanini (`@MarcoBonzanini <http://www.twitter.com/marcobonzanini>`_)
- Miguel Martinez-Alvarez (`@MiguelMAlvarez <http://www.twitter.com/miguelmalvarez>`_)

Slides
-----

PyCon UK 2016 Tutorial: `presentations/pyconuk-slides.pdf`

License
-----

Code (mainly in `notebooks` folder) under MIT license.

Documentation and slides under CC-BY license.

Data
-----

- Documents in `data/recipes` are public domain from Project Gutenberg
- Documents in `data/pyconuk2016` are the abstracts from https://github.com/PyconUK/2016.pyconuk.org

