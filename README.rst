.. image:: https://travis-ci.org/vmware/pyvmomi.svg?branch=v6.0.0.2016.4
    :target: https://travis-ci.org/vmware/pyvmomi
    :alt: Build Status

.. image:: https://img.shields.io/pypi/dm/pyvmomi.svg
    :target: https://pypi.python.org/pypi/pyvmomi/
    :alt: Downloads

pyVmomi is the Python SDK for the VMware vSphere API that allows you to manage 
ESX, ESXi, and vCenter.

Getting Started
================
To get started, see the `getting started guide <http://vmware.github.io/pyvmomi-community-samples/#getting-started>`_. You'll need `Python <https://www.python.org/downloads/>`_, `pip <https://pip.pypa.io/en/latest/installing.html#using-package-managers>`_, and the `samples project <https://github.com/vmware/pyvmomi-community-samples/tarball/master>`_.

* http://vmware.github.io/pyvmomi-community-samples/
* community discussion on IRC freenode.net channels `#pyvmomi and #pyvmomi-dev <http://webchat.freenode.net/?channels=#pyvmomi,#pyvmomi-dev>`_
* community email is on `nabble <http://pyvmomi.2338814.n4.nabble.com>`_

Don't know what pip is? Any serious python developer should know, so here's a `throrough intro to pip <http://www.dabapps.com/blog/introduction-to-pip-and-virtualenv-python/>`_ that we like.

Installing
==========
The master is code that is in development, official releases are tagged and 
posted to `pypi <https://pypi.python.org/pypi/pyvmomi/>`_

* The official release is available using pip, just run 
  ``pip install --upgrade pyvmomi``. 
* To install the version in `github <https://github.com/vmware/pyvmomi>`_ use 
  ``python setup.py develop`` for development install or 
  ``python setup.py install``.
* To install `github's version <https://github.com/vmware/pyvmomi>`_ with sso support, just run
  ``pip install -e .[sso]`` inside project's home folder.

Testing
=======
Unit tests can be invoked by using the `tox <https://testrun.org/tox/>`_ command. You may have to
configure multiple python interpreters so that you can test in all the
environments listed in ``tox.ini`` or you will have to run ``tox`` with the
``-e`` flag to run only in your version of python. For example, if you only
have Python 2.7 then ``tox -e py27`` will limit your test run to Python 2.7.

Contributing
============
* Research `open issues <https://github.com/vmware/pyvmomi/issues?q=is%3Aopen+is%3Aissue>`_
* Follow the `contribution standards <https://github.com/vmware/pyvmomi/wiki/Contributions>`_
* Coordinate with `other developers <http://webchat.freenode.net/?channels=#pyvmomi,#pyvmomi-dev>`_ on the project.

Documentation
=============
For general language neutral documentation of vSphere Management API see: 

* `vSphere WS SDK API Docs <https://code.vmware.com/apis/968/vsphere>`_

Python Support
==============
* pyVmomi supports 2.7.x and 3.4+

Note: python2 is deprecated from 01/2020 https://www.python.org/doc/sunset-python-2/. Please switch to Python3 

Compatibility Policy
====================
pyVmomi versions are marked vSphere_version-release . Pyvmomi maintains minimum 
backward compatibility with the previous _four_ releases of *vSphere* and it's 
own previous four releases. Compatibility with much older versions may continue 
to work but will not be actively supported.

For example, version v6.0.0 is most compatible with vSphere 6.0, 5.5, 5.1 and
5.0. Initial releases compatible with a version of vSphere will bare a naked
version number of v6.0.0 indicating that version of pyVmomi was released
simultaneously with the *GA* version of vSphere with the same version number.

Related Projects
================
* VMware vSphere Automation SDK for Python: https://github.com/vmware/vsphere-automation-sdk-python
* Samples Project: https://github.com/vmware/pyvmomi-community-samples

Have fun!
