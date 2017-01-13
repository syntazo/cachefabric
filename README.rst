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

.. |docs| image:: https://readthedocs.org/projects/cachefabric/badge/?version=latest
    :target: http://cachefabric.readthedocs.io/en/latest/?badge=latest
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

.. |codacy| image:: https://api.codacy.com/project/badge/Grade/0a935a0e64764ac5bee4c4f73d405e95    
    :target: https://www.codacy.com/app/thanos/cachefabric?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=syntazo/cachefabric&amp;utm_campaign=Badge_Grade
    :alt Codacy Tests
    
    
.. |codeclimate| image:: https://codeclimate.com/github/syntazo/cachefabric/badges/gpa.svg
   :target: https://codeclimate.com/github/syntazo/cachefabric
   :alt: Code Climate

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




What is CacheFabric ?
=====================

Free & open source, high-performance, distributed p2p memory object caching system, generic in nature, but intended for use in speeding up dynamic applications by alleviating database load, data transferload by keeping what you need local.

CacheFabric is a drop-in replacement for memcached

CacheFabric is simple yet powerful. Its simple design promotes quick deployment, ease of development, and solves many problems facing large data caches. Its API is available for most popular languages.



* Distributed Cache
* Hot/Cold Data locality control
* Arcoss Data centers
* Eventual Consistancy
* Native memory storage avoids garbage collection and provides predictable low latency across different applications without affecting each other
* Java, .NET and C++ applications can use native client libraries to access the cache. For other languages, applications can use Hazelcast REST and Memcached interfaces
* CacheFabric   lets you monitor cache server nodes, connected clients, and used caches. It will now give notification when certain cluster management operations take too long, helping to identify performance and stability issues.
* WAN Replication lets you replicate the cache across multiple data centers.
* JCache and Map Interfaces are two standard APIs provided by CacheFabric. JCache is standard for JSR 107 and Map Interface is based on java.util.Map
* MapStore and CacheStore, respectively for Map and JCache, can be used to make CacheFabric automatically load and store data from a database
* CacheFabric High Density Memory Store (HDMS) for Near Cache (behind the JCache API) allows each app server to store hundreds of GB of cached data in memory locally (as opposed to the ~3.5 GB practical limit for on-heap data).
* High Density Memory Store for Near Cache allows each app server to access data faster: in microseconds instead of milliseconds.
* Cache-as-a-service can be updated independently of the applications (for minor-version updates). Applications using cache-as-a-service don’t need to upgrade in lock-step when cache-as-a-service is patched or upgraded, making cache-as-a-service much easier to use and giving independent applications more autonomy.



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
