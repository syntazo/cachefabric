========
Overview
========

.. start-badges

.. list-table::
    :stub-columns: 1

    * - docs
      - |docs|
    * - tests
      - | |travis| 
        | |coveralls| |codecov|
        | |landscape|  |codacy| |codeclimate|
    * - package
      - |version| |downloads| |wheel| |supported-versions| |supported-implementations|

.. |docs| image:: https://readthedocs.org/projects/cachefabric/badge/?style=flat
    :target: https://readthedocs.org/projects/cachefabric
    :alt: Documentation Status

.. |travis| image:: https://travis-ci.org/syntazo/cachefabric.svg?branch=master
    :alt: Travis-CI Build Status
    :target: https://travis-ci.org/syntazo/cachefabric


.. |coveralls| image:: https://coveralls.io/repos/github/syntazo/cachefabric/badge.svg?branch=master
    :alt: Coverage Status
    :target: https://coveralls.io/github/syntazo/cachefabric?branch=master
    


.. |codecov| image:: https://codecov.io/gh/syntazo/cachefabric/branch/master/graph/badge.svg
    :alt: Coverage Status  
    :target: https://codecov.io/gh/syntazo/cachefabric

.. |landscape| image:: https://landscape.io/github/syntazo/cachefabric/master/landscape.svg?style=flat
   :target: https://landscape.io/github/syntazo/cachefabric/master
   :alt: Code Health    

.. |codacy| image:: https://img.shields.io/codacy/REPLACE_WITH_PROJECT_ID.svg?style=flat
    :target: https://www.codacy.com/app/thanos/cachefabric
    :alt: Codacy Code Quality Status

.. |codeclimate| image:: https://codeclimate.com/github/thanos/cachefabric/badges/gpa.svg
   :target: https://codeclimate.com/github/thanos/cachefabric
   :alt: CodeClimate Quality Status

.. |version| image:: https://img.shields.io/pypi/v/cachefabric.svg?style=flat
    :alt: PyPI Package latest release
    :target: https://pypi.python.org/pypi/cachefabric

.. |downloads| image:: https://img.shields.io/pypi/dm/cachefabric.svg?style=flat
    :alt: PyPI Package monthly downloads
    :target: https://pypi.python.org/pypi/cachefabric

.. |wheel| image:: https://img.shields.io/pypi/wheel/cachefabric.svg?style=flat
    :alt: PyPI Wheel
    :target: https://pypi.python.org/pypi/cachefabric

.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/cachefabric.svg?style=flat
    :alt: Supported versions
    :target: https://pypi.python.org/pypi/cachefabric

.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/cachefabric.svg?style=flat
    :alt: Supported implementations
    :target: https://pypi.python.org/pypi/cachefabric




.. end-badges

high-performance, distributed p2p persistant cache - the technology behind data fabric

* Free software: BSD license

Installation
============

::

    pip install cachefabric

Documentation
=============

https://cachefabric.readthedocs.io/

Development
===========

To run the all tests run::

    tox

Note, to combine the coverage data from all the tox environments run:

.. list-table::
    :widths: 10 90
    :stub-columns: 1

    - - Windows
      - ::

            set PYTEST_ADDOPTS=--cov-append
            tox

    - - Other
      - ::

            PYTEST_ADDOPTS=--cov-append tox
