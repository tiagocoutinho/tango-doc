
.. _start:

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

  * Download and install ZMQ (zeromq_).
  
.. _zeromq: https://archive.org/download/zeromq_4.0.7/zeromq-4.0.7.tar.gz

    The default installation directory is /usr/local but you can override this with the --prefix option.
    Beware versions >4.0.7 require libsodium to be installed. ::

    $ tar xvf zeromq-4.0.7.tar.gz
    $ cd zeromq-4.0.7/
    $ ./configure --prefix=/usr/local
    $ make
    $ sudo make install


  * Download and install omniORB_ ::

    $ tar xvf omniORB-4.2.1-2.tar.bz2
    $ cd omniORB-4.2.1
    $ ./configure --prefix=/usr/local
    $ make
    $ sudo make install

.. _omniORB: https://sourceforge.net/projects/omniorb/files/omniORB/omniORB-4.2.1/omniORB-4.2.1-2.tar.bz2/download

  * Install MySQL ::

    $ todo

  Finally download the tango_ source. It is recommended to create a build directory if you need to install for more than one platform. ::

   $ tar xvf tango-9.2.2.tar.gz
   $ mkdir tango-9.2.2-build-x86_64
   $ cd tango-9.2.2-build-x86_64
   $ ../tango-9.2.2/configure --prefix=/usr/local --with-mysql-admin=root --with-mysql-admin-password= --with-mysqlclient-lib=/usr/lib64/mysql
   $ make
   $ sudo make install

.. _tango: https://sourceforge.net/projects/tango-cs/files/tango-9.2.2.tar.gz/download

The virtual machine
+++++++++++++++++++

  Andy you said you had some words for this

A Debian package
++++++++++++++++
   
   need to try this 


Windows
~~~~~~~

   Anyone?


