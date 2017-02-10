PyTango Meeting: minutes
============================
**Febuary 6th 2017 **


Pytango server restart segfault
-------------------------------
 - Tiago has a good idea of what this bug can be about.

> -> This should be documented in a github issue.

 - Still low priority

Fix using deprecated NumPy API
------------------------------
 - This seems to have been solved by Carlos.

> -> We should ask him about this issue and create a PR

 - Other compilation warnings are related to zero message queue.

> -> We should investigate those warnings and probably report them on the cppTango github



Get rid of metaclass definition
-------------------------------
  - It is done and released on pytango 9.2.1


Continuous integration
----------------------
 - Travis uses conda to run PyTango unitest.

>   -> There is no official Tango channel in Conda

>   -> Travis could build this Conda package.
 
 - Conda might make Windows builds easier.


Define git workflow
-------------------
> -> Make develop branch as default branch in github



Documentation generation
------------------------
 - The PyTango ESRF website is still the default result in Google
>   -> we should create a link on this URL to the official ReadTheDoc website.

 - Old PyTango documentations (PyTango version < 9.) are not hosted on RTD and should stay on the ESRF servers.

 - There is no documentation about documentation generation and mock system.

 - PyTango documentation needs to be reviewed:

>   -> Make documentation up to date

>   -> Promote HL API as the default way of programming in Python.

>   -> Document and promote new features.

 - There is a plan to improve documentation on cpptango side (task force), we should harmonize and include pytango in the task force.

  
Change of binding
-----------------
 - It is a huge effort.

 - Alternative:
     - sip
     - cython
     - pybind11 (close to boost)
     - pure python binding.
   
 - It is probably better to wait Tango10 before starting something.

 - We have to keep track of what is going on in cppTango to avoid issue with the current PyTango boost implementation.

 - Build tango for windows is difficult due to boost. It has been handled by Sebastien Gara for PyTango 9.2.0.

 
Move itango to separate project
-------------------------------
 - itango documentation is not on readthedoc but on pythonhosted

 - Nicolas Leclerq has done an example of what can be done today with Jupyter, Ipywidgets, Bokeh that can be combined with itango.


Refactor setup.py
-----------------
 - Requierement are now supported with pip.

Server argparse
---------------
 - Extend PyTango command line interface and add custom argument.
 - Issue: corba argument are not fully compatible with argparse.
 - Low priority because it is not compatible with the starter.
 - It can be a good task to get in PyTango for some who wants to start contributing.

Rename PyTango to tango
-----------------------
 - We should write somthing in documentation about this renaming.

Refactor asynchronous layer
---------------------------
 - We still have to isolate gevent and asyncio.

Define coding standards
-----------------------
 - Add guide line in documentation about coding standards

Clean up
--------------------
 - Keep old object for backward compatibility and advertise HL API.
 - There is a lot of attributes expose in the tango module. We should clean up at the next major realise and advertise for compatiblity

