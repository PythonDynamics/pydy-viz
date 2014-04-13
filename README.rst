pydy-viz
========

**Notice**

**pydy-viz has been merged into the main pydy repository. This independent
project is now deprecated, all development and subsequent releases will be from
http://github.com/pydy/pydy.**

Visualization of multibody systems generated with PyDy.

Installation
============

This package relies on dependencies included in the SciPy stack (i.e. NumPy and
matplotlib). These packages are not necessarily easy to install from source, so
it is best to follow the instructions available on the `SciPy installation
page`_.

.. _SciPy installation page: http://www.scipy.org/install.html

One example of installing the setuptools, NumPy, and matplotlib dependencies
for Debian based Linux systems is to install from the apt package manager::

   $ apt-get install python-setuptools python-numpy python-matplotlib

Once the dependencies are installed, then download the source and install with::

   $ python setup.py install

This will automatically install the latest version of the final dependency
SymPy if needed.

**Note that pydy-viz is currently only tested on Python 2.7.**

Tests
=====

The Python tests require nose so get them with your package manager::

   $ apt-get python-nose python-coverage

or pip::

   $ pip install nose coverage

The tests can be run from the root directory with::

   $ nosetests

And to see more detail with coverage, run::

   $ nosetests -v --with-coverage --cover-package=pydy_viz

These are alternative ways to run the Python tests::

   $ bin/test
   $ python setup.py nosetests


Documentation
=============

The documentation is hosted at http://pydy-viz.readthedocs.org but you can also
build them from source using the following instructions:

Requires:

- Sphinx
- numpydoc

::

   pip install sphinx numpydoc

To build the HTML docs::

   $ sphinx-build -b html docs/src docs/build

View::

   $ firefox docs/build/index.html

Release Notes
=============

0.1.0
-----

- Initial release.
