Pyxshell Documentation
======================

Pyxshell aims to bring bash-style pipelining to Python generators.

A short example::

    >>> from pyxshell.common import grep,glue
    >>> pl = []
    >>> ['python', 'ruby', 'jython'] | grep(r'yt') > pl
    >>> pl | glue("\n") > sys.stdout
    python
    jython

To see some examples of simple but useful pipeline components, check out the
:mod:`pyxshell.common` module. To get started writing your own, read the
:class:`~pyxshell.pipeline` documentation.

Installation
------------

You can get the module from PyPI::

    pip install pyxshell


Table of Contents
-----------------

.. toctree::
    :maxdepth: 2

    pipeline
    common
