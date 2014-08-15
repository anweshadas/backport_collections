backport_collections
====================

.. image:: https://badge.fury.io/py/backport_collections.png
    :target: http://badge.fury.io/py/backport_collections

.. image:: https://travis-ci.org/sk-/backport_collections.png?branch=master
    :target: https://travis-ci.org/sk-/backport_collections

.. image:: https://coveralls.io/repos/sk-/backport_collections/badge.png?branch=master
    :target: https://coveralls.io/r/sk-/backport_collections?branch=master

backport_collections is a backport of Python 2.7's ``collections`` module for Python 2.6 and 2.5.

What is backported?
-------------------

``Counter``, ``OrderedDict`` and ``namedtuple`` are backported.

Usage
-----

To use it just import the desired classes from the module ``backport_collections``.
Example::

    from backport_collections import Counter
    from backport_collections import OrderedDict
    from backport_collections import namedtuple

Known Issues
------------

* In Python 2.6 Issue 9137 is not solved as it complains if it gets a keyword
argument named ``self``. The error is ``TypeError: update() got multiple values for keyword argument 'self'``.

License
-------

The Python Software Foundation License.

Changes
-------

* v0.1 (15/08/2014): Synced to revision http://hg.python.org/cpython/rev/6d41f139709b