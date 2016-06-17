
.. _start:

.. toctree::
   :maxdepth: 2


Getting started
===============

Installing
----------

Linux
~~~~~

  Tango is available on linux as:

  * as source code sourceforge
  * as a virtual machine
  * as an official debian package


Compiling the source code
+++++++++++++++++++++++++

  There are 3 pre-requisites to building the Tango source code

  * Download and install ZMQ (zeromq). 

    The default installation directory is /usr/local but you can override this with the --prefix option.
    Beware versions >4.0.7 require libsodium to be installed. ::

    $ tar xvf zeromq-4.0.7.tar.gz
    $ cd zeromq-4.0.7/
    $ ./configure --prefix=/usr/local
    $ make
    $ sudo make install


  * Download and install omniORB ::

    $ tar xvf omniORB-4.2.1-2.tar.bz2
    $ cd omniORB-4.2.1
    $ ./configure --prefix=/usr/local
    $ make
    $ sudo make install

  * Install MySQL ::

    $ todo

  Finally download the tango source. It is recommended to create a build directory if you need to install for more than one platform. ::

   $ tar xvf tango-9.1.0.tar.gz
   $ mkdir tango-9.1.0-build-x86_64
   $ cd tango-9.1.0-build-x86_64
   $ ../tango-9.1.0/configure --prefix=/usr/local --with-mysql-admin=root --with-mysql-admin-password= --with-mysqlclient-lib=/usr/lib64/mysql
   $ make
   $ sudo make install

The virtual machine
+++++++++++++++++++

  Andy you said you had some words for this

A Debian package
++++++++++++++++
   
   need to try this 


Windows
~~~~~~~

   Anyone?


