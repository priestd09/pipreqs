===============================
``pipreqs`` - Generate requirements.txt file for any project based on imports
===============================

.. image:: https://img.shields.io/travis/bndr/pipreqs.svg
        :target: https://travis-ci.org/bndr/pipreqs
      
        
.. image:: https://img.shields.io/pypi/v/pipreqs.svg
        :target: https://pypi.python.org/pypi/pipreqs

.. image:: https://img.shields.io/pypi/dm/pipreqs.svg
        :target: https://pypi.python.org/pypi/pipreqs
        
.. image:: https://img.shields.io/coveralls/bndr/pipreqs.svg 
        :target: https://coveralls.io/r/bndr/pipreqs
  
        
.. image:: https://img.shields.io/pypi/l/pipreqs.svg 
        :target: https://pypi.python.org/pypi/pipreqs

        

Installation
------------

::

    pip install pipreqs

Usage
-----

::

    Usage:
        pipreqs [options] <path>

    Options:
        --debug             Print debug information
        --savepath <file>   Save the list of requirements in the given file

Example
-------

::

    $ pipreqs /home/project/location
    Looking for imports
    Getting latest information about packages from PyPI
    Found third-party imports: flask, requests, sqlalchemy, docopt
    Successfully saved requirements file in /home/project/location/requirements.txt
 
Why not pip freeze?
-------------------

- ``pip freeze`` only saves the packages that are installed with ``pip install`` in your environment. 
- pip freeze saves all packages in the environment including those that you don't use in your current project. (if you don't have virtualenv)
- and sometimes you just need to create requirements.txt for a new project without installing modules.
