=============
Installation
=============
This is a step by step guide to install and run Sitar on you system.


Prerequisites
--------------

- Linux (tested on Ubuntu 12:04)
- gcc >= version 4.5
- python >= version 2.7
- scons
- OpenMP (optional) Required for parallel simulation.


Install scons
^^^^^^^^^^^^^^

.. code-block:: bash

    $ python -m pip install scons


Install OpenMP
^^^^^^^^^^^^^^

.. code-block:: bash

    $ sudo apt-get install libomp-dev


INSTALLATION INSTRUCTIONS (FOR LINUX)
--------------------------------------

**Step 1 :**

Run install.py

.. code-block:: bash

    $ python install.py

or



.. code-block:: bash

    $ python3 install.py

**Setp 2 :** 

Add the following lines to your ~/.bashrc file
to use the sitar translator and compiler executables
outside the installation folder. Replace <path> 
with absolute path of this folder.

.. code-block:: bash

    #sitar paths:
    export LD_LIBRARY_PATH=<path-to-sitar>/translator/antlr3Cruntime/build/lib:${LD_LIBRARY_PATH}
    export PATH=<path-to-sitar>/scripts:${PATH}












