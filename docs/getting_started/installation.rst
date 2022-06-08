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


**Install scons**

.. code-block:: bash

    $ python -m pip install scons


**Install OpenMP (optional)**

.. code-block:: bash

    $ sudo apt-get install libomp-dev


INSTALLATION INSTRUCTIONS (FOR LINUX)
--------------------------------------

**Step 1 :**
Clone the `sitar repository
<https://github.com/NehaKaranjkar/sitar>`_ and go to sitar folder byt running the following command in your terminal.

.. code-block:: bash

    git clone git@github.com:NehaKaranjkar/sitar.git
    cd sitar


**Step 2 :**
Run install.py in terminal.

.. code-block:: bash

    $ python install.py

or

.. code-block:: bash

    $ python3 install.py

**Setp 3 :** 
Add the following lines to your ~/.bashrc file
to use the sitar translator and compiler executables
outside the installation folder. Replace <path> 
with absolute path of this folder.

.. code-block:: bash

    #sitar paths:
    export LD_LIBRARY_PATH=<path-to-sitar>/translator/antlr3Cruntime/build/lib:${LD_LIBRARY_PATH}
    export PATH=<path-to-sitar>/scripts:${PATH}

**Step 4 :**
Check if Sitar is successfull installed by running the following command in your terminal.

.. code-block:: bash

    sitar -h

This should list the available sitar commands.












