========
Overview
========

.. start-badges

.. list-table::
    :stub-columns: 1

    * - docs
      - |docs|
    * - tests
      - | |travis| |appveyor| |requires|
        | |coveralls| |codecov|
        | |landscape| |scrutinizer| |codacy| |codeclimate|
    * - package
      - |version| |downloads| |wheel| |supported-versions| |supported-implementations|

.. |docs| image:: https://readthedocs.org/projects/cachefabric/badge/?style=flat
    :target: https://readthedocs.org/projects/cachefabric
    :alt: Documentation Status

.. |travis| image:: https://travis-ci.org/thanos/cachefabric.svg?branch=master
    :alt: Travis-CI Build Status
    :target: https://travis-ci.org/syntazo/cachefabric

.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/thanos/cachefabric?branch=master&svg=true
    :alt: AppVeyor Build Status
    :target: https://ci.appveyor.com/project/thanos/cachefabric

.. |requires| image:: https://requires.io/github/thanos/cachefabric/requirements.svg?branch=master
    :alt: Requirements Status
    :target: https://requires.io/github/thanos/cachefabric/requirements/?branch=master

.. |coveralls| image:: https://coveralls.io/repos/thanos/cachefabric/badge.svg?branch=master&service=github
    :alt: Coverage Status
    :target: https://coveralls.io/r/thanos/cachefabric

.. image:: https://codecov.io/gh/syntazo/cachefabric/branch/master/graph/badge.svg
    :alt: Coverage Status  
    :target: https://codecov.io/gh/syntazo/cachefabric

.. |landscape| image:: https://landscape.io/github/thanos/cachefabric/master/landscape.svg?style=flat
    :target: https://landscape.io/github/thanos/cachefabric/master
    :alt: Code Quality Status

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

.. |scrutinizer| image:: https://img.shields.io/scrutinizer/g/thanos/cachefabric/master.svg?style=flat
    :alt: Scrutinizer Status
    :target: https://scrutinizer-ci.com/g/thanos/cachefabric/


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
