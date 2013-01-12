:mod:`~pyxshell.common`
=========================

:mod:`pyxshell.common` defines some helpful pipeline components, borrowed
straight from UNIX but adapted to work with arbitrary Python objects instead of
just simple text streams.

For example, the following list of functions can be grabbed with::

    >>> from pyxshell.common import *
    >>> ("    *    :func:`%s`"%c for c in cat("pyxshell/common.py") | grep("def") | cut(1) | cut(0,"(") | filter(lambda i:"default" not in i) | uniq ) | sort() | glue("\n") > sys.stdout

.. automodule:: pyxshell.common
    :members:

    Defined in this module:
    *    :func:`cat`
    *    :func:`curl`
    *    :func:`cut`
    *    :func:`dir_file`
    *    :func:`dos2unix`
    *    :func:`echo`
    *    :func:`expand`
    *    :func:`filter`
    *    :func:`glue`
    *    :func:`grep_e`
    *    :func:`grep_in`
    *    :func:`grep`
    *    :func:`head`
    *    :func:`join`
    *    :func:`map`
    *    :func:`pretty_printer`
    *    :func:`sed`
    *    :func:`sh`
    *    :func:`sort`
    *    :func:`tail`
    *    :func:`tee`
    *    :func:`traverse`
    *    :func:`uniq`
    *    :func:`unix2dos`
    *    :func:`wc`

