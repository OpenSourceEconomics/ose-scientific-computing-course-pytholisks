
Summary of OSE Scientific Computing Project on `pydsge` (by Yuxin, Altaf and Philipp)
======

.. image:: https://img.shields.io/github/workflow/status/OpenSourceEconomics/ose-scientific-computing-course-pytholisks/Continuous%20Integration%20Workflow?label=Continuous%20Integration&logo=github
    :target: https://github.com/OpenSourceEconomics/ose-scientific-computing-course-pytholisks//actions?query=branch%3Aimplementing_CI

Testing with pytest
-------------
 - A testing suite for regression testing of the tutorial(s) was created
 - A preliminary test against a closed form solution of a smaller model was created
 - A basic test of the parser was created

 Multiprocessing on Windows
-------------
 - A pull-request with the relevant changes was created for grglib
 - Gregor’s simplifications were adopted
 - for documentation purposes and Prof. Eisenhauer, full details are provided in `Summary.pdf <https://docs.google.com/document/d/1kWifKdqk_KpfPecELgSkH08Cj23xyQV2hYSu_m4Rjg0/edit?usp=sharing>`

Estimation Tutorial
-------------
 - An estimation tutorial for pydsge was created based on a script provided by Gregor
 - Several issues that were discovered in the process were fixed, documentation was improved

Pre-commit check of Code style
-------------
 - A pre-commit hook was created which, among others, includes black, blacken and flake8 (with several adjustments)

Continuous Integration Workflow
-------------
 - To enable cross-platform and cross-version code control and maintenance, a github CI workflow for Unix, MacOs and Windows as well as Python 3.8 and 3.9 was created. (Having a specific  badge for these environments would require Anaconda)
 - The CI workflow runs the pytest framework and, if needed, can be set to update the pickle used for the tests (Ubuntu with python 3.8 is used as the stable version.)





----

Contains the functions and classes for solving, filtering and estimating DSGE models at the ZLB (or with other occasionally binding constraints).

A collection of models that can (and were) used with this package can be found in `another repo <https://github.com/gboehl/projectlib/tree/master/yamls>`_.

The code is in alpha state and provided for reasons of collaboration, replicability and code sharing in the spirit of open science. It does not (and for now, can not) have a toolbox character. The code is operational, but (yet) not ready for public use and I can not provide any support. You are however very welcome to get in touch if you are interested working with the package.

Installation
-------------

Installing the repo version is as simple as

.. code-block:: bash

   pip install pydsge

Documentation
-------------

There is some `preliminary documentation <https://pydsge.readthedocs.io/en/latest/index.html>`_ out there.

- `Installation Guide <https://pydsge.readthedocs.io/en/latest/installation_guide.html>`_
- `Getting Started <https://pydsge.readthedocs.io/en/latest/getting_started.html>`_
- `Module Documentation <https://pydsge.readthedocs.io/en/latest/modules.html>`_

Citation
--------

**pydsge** is developed by Gregor Boehl to simulate, filter, and estimate DSGE models with the zero lower bound on nominal interest rates in various applications (see `my website <https://gregorboehl.com>`_ for research papers using the package). Please cite it with

.. code-block::

    @techreport{boehl2021method,
      Title = {Efficient Solution and Computation of Models with Occasionally Binding Constraints},
      Author = {Gregor Boehl},
      Year = {2021},
      institution = {Goethe University Frankfurt, Institute for Monetary and Financial Stability (IMFS)},
      type = {IMFS Working Paper Series},
      number = {148},
      url = {https://gregorboehl.com/live/obc_boehl.pdf},
    }

We appreciate citations for **pydsge** because it helps us to find out how people have
been using the package and it motivates further work.


Parser
------

The parser originally was a fork of Ed Herbst's fork from Pablo Winant's (excellent) package **dolo**. 

See https://github.com/EconForge/dolo and https://github.com/eph.


References
----------

Boehl, Gregor (2021). `Efficient Solution and Computation of Models with Occasionally Binding Constraints <http://gregorboehl.com/live/obc_boehl.pdf>`_. *IMFS Working Paper*
