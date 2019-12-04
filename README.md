﻿jk_mounting
===========

Introduction
------------

This python module provides support for mounting/unmounting and retrieving mounting information.

Information about this module can be found here:

* [github.org](https://github.com/jkpubsrc/python-module-jk-mounting)
* [pypi.python.org](https://pypi.python.org/pypi/jk_mounting)

How to use this module
----------------------

### Import

To import this module use the following statement:

```python
import jk_mounting
```

### Retrieve Information

In order to get information about what kind of devices are mounted, use the following command:

```python
mounter = jk_mounting.Mounter()

for mi in mounter.getMountInfos(isRegularDevice = True):
	print(mi)
```

### Mount a Device

To mount a device you can use the following command:

```python
mounter = jk_mounting.Mounter()

mounter.mount("/dev/sdd1", "/mnt")
```

Contact Information
-------------------

This is Open Source code. That not only gives you the possibility of freely using this code it also
allows you to contribute. Feel free to contact the author(s) of this software listed below, either
for comments, collaboration requests, suggestions for improvement or reporting bugs:

* Jürgen Knauth: jknauth@uni-goettingen.de, pubsrc@binary-overflow.de

License
-------

This software is provided under the following license:

* Apache Software License 2.0



