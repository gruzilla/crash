=================
The CrateDB Shell
=================

.. image:: https://travis-ci.org/crate/crash.svg?branch=master
    :target: https://travis-ci.org/crate/crash
    :alt: Travis CI

.. image:: https://badge.fury.io/py/crash.svg
    :target: http://badge.fury.io/py/crash
    :alt: Version

.. image:: https://img.shields.io/badge/docs-latest-brightgreen.svg
    :target: https://crate.io/docs/reference/crash/
    :alt: Documentation

.. image:: https://coveralls.io/repos/github/crate/crash/badge.svg?branch=master
    :target: https://coveralls.io/github/crate/crash?branch=master
    :alt: Coverage

|

The CrashDB Shell (aka *Crash*) is an interactive *command line interface*
(CLI) for CrateDB.

Screenshot
==========

.. image:: https://raw.githubusercontent.com/crate/crash/master/crash.png
    :alt: A screenshot of Crash

Prerequisites
=============

Recent versions of Crash require Python 3 (>= 3.4) to run.

Use Crash version 0.23.x if you are running Python 2.7 or 3.3.

Use Crash version 0.16.x if you're running Python 2.6.

Installation
============

Under normal circumstances, you do not have to manually install Crash.

Crash is bundled with CrateDB.

If you are able to run the ``crate`` command, you should be able to run the
``crash`` command (either from the same ``bin`` directory, or on your `PATH`_).

The following instructions should only be followed if you specifically want to
install Crash separately from CrateDB.

As a Python Package
-------------------

Crash is available as a pip_ package.

To install, run::

    $ pip install crash

Now, run it::

    $ crash

To update, run::

    $ pip install -U crash

If you are not using Python version 3.4 or above, recent version of pip_ will
only install version 0.23.x. This is because newer versions of this package are
not compatible with Python 2.7 or 3.3 and below.

Standalone
----------

Crash is also available as a standalone executable that includes all the
necessary dependencies, and can be run as long as Python (>= 3.4) is available
on your system.

First, download the executable file::

    $ curl -o crash https://cdn.crate.io/downloads/releases/crash_standalone_latest

Then, set the executable bit::

    $ chmod +x crash

Now, run it::

    $ ./crash

If you would like to run ``crash`` from any directory and without using leading
``./`` you will need to move it to somewhere on your ``$PATH``.

Legacy Versions
...............

For Python 2.7 and 3.3 please download version ``0.23.0`` from the CDN::

    $ curl -o crash https://cdn.crate.io/downloads/releases/crash_standalone_0.23.0

For Python 2.6 please download version ``0.16.2`` from the CDN::

    $ curl -o crash https://cdn.crate.io/downloads/releases/crash_standalone_0.16.2

Usage
=====

For usage information and options, run::

    $ crash --help

Contributing
============

This project is primarily maintained by Crate.io_, but we welcome community
contributions!

See the `developer docs`_ and the `contribution docs`_ for more information.

Help
====

Looking for more help?

- Read `the project documentation`_
- Check `StackOverflow`_ for common problems
- Chat with us on `Slack`_
- Get `paid support`_

.. _contribution docs: CONTRIBUTING.rst
.. _Crate.io: http://crate.io/
.. _developer docs: DEVELOP.rst
.. _paid support: https://crate.io/pricing/
.. _pip: https://pypi.python.org/pypi/pip
.. _Slack: https://crate.io/docs/support/slackin/
.. _StackOverflow: https://stackoverflow.com/tags/crate
.. _the project documentation: https://crate.io/docs/reference/crash/
.. _PATH: https://en.wikipedia.org/wiki/PATH_(variable)
