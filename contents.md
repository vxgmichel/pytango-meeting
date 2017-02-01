name: empty layout
layout: true

---
name: main title
class: center, middle

Pytango progress report
=======================

Vincent Michel @ MAX-IV

Pytango meeting 2017 - ESRF

---
name: main issue layout
layout: true

1. Main issues
==============

---

Pytango server restart segfault
-------------------------------

- Urgency: medium/low
- Difficulty to solve: hard
- **Postponed**

Fix using deprecated NumPy API
------------------------------

- Urgency: low
- Difficulty to solve: hard
- **Status?**

Get rid of metaclass definition
-------------------------------

- **Done**: Fix by PR#90, visible in 9.2.1

---
name: major task layout
layout: true

2. Major tasks
==============

---

| Tasks                           | Status                    |
|---------------------------------|---------------------------|
| Unit tests                      | **Done, to be improved**  |
| Continuous integration          | **Done**                  |
| Define git workflow             | **Done, to be discussed** |
| Documentation generation        | **Done**                  |
| Change of binding               | **Postponed**             |
| Move itango to separate project | **Done**                  |
| Refactor setup.py               | **Done, to be improved**  |
| Server argparse                 | **Postponed**             |
| Rename PyTango to tango         | **Done, following up**    |
| Refactor asynchronous layer     | **Ongoing**               |
| Refactor tango objects          | **Done**                  |
| Define coding standards         | **Ongoing**               |
| Clean directory tree            | **Done**                  |
| Simplify DeviceImpl             | **Done, to be discussed** |
| Releases                        | **Done, following up**    |

---

Unit tests
----------

**Done:**
- Basic server tests
- Very basic client tests
- Very basic event tests

**Improvements:**
- MOAR TESTS!

**Issues:**
- Constantly fighting tango limitation
- No code coverage

---

Continuous integration
----------------------

**Done:**
- TravisCI is running tests in a conda environment

**To discuss:**
- Shoud Travis build conda packages?

---

Define git workflow
-------------------

**Done:**
- PR -> develop -> master seems to work fine

**To discuss:**
- Should we document it?
- Should we make develop the default branch?

---

Documentation generation
------------------------

**Done:**
- The documentation is now hosted on readthedocs

**How:**
- Heavy mocking... is that an issue?

**Issue:**
- Only works with >= python3.5

---

Change of binding
-----------------

**=> Postponed**

Move itango to separate project
-------------------------------

**Done:**
- Move to tango-controls/itango
- Compatibility package 0.0.1

**Issue:**
- Backward compatibility is a mess

---

Refactor setup.py
-----------------

**Done:**
- Link with specific tango .so file
- Use setuptools
- Refactor platform specific code
- Add classifiers and requirements

Server argparse
---------------

**=> Postponed**

---

Rename PyTango to tango
-----------------------

**Done:**
- The module is now called tango
- A PyTango compatibilty module has been added

**To do:**
- Issue warnings?

---

Refactor asynchronous layer
---------------------------

**Done:**
- Some parts of it
- Bug fixes

**Remaining:**
- Define a unified client/server abstract interface for executors

---

Refactor tango objects
----------------------

**Done:**
- Move tango objects to a separate module

Define coding standards
-----------------------

**Done:**
- Many modules have been PEP8-ified

**Remaining:**
- Write guidelines
- Maybe a "contribute" section?

---

Clean directory tree
--------------------

**Done:**
- Most of the unused files have been removed from pytango 9
- But still available in the tango8 branch

Simplify DeviceImpl
-------------------

**Done:**
- LatestDeviceImpl is the only documented class

**To discuss:**
- Should LatestDeviceImpl be the only DeviceImpl?

---

Releases
--------

**Done:**
- Version 8.1.9 - 12/08/2016
- Version 9.2.0 - 18/08/2016
- Version 9.2.1 - 30/01/2016


---
name: discussion layout
layout: true

3. Discussion
=============

---
name: final
layout: false
class: center, middle

Presentation written in `Markdown` and rendered by [remark](http://remarkjs.com/) slideshow tool

Sources for this presentation can be found on github

[vxgmichel/presentation-pytango-quality](https://github.com/vxgmichel/pytango-meeting)

Thanks
