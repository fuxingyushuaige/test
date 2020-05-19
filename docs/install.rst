Installation
==================

Dependencies
+++++++++++++++

We highly recommend installing this package using the ``conda`` utility to ensure all dependencies are loaded with their correct versions. We provide a wdtools.yaml file in the root directory of our GitHub repository. To create a new ``conda`` environment with all dependencies, use the following code:

.. code-block:: bash

   conda env create -f wdtools.yaml
   conda activate wdtools

This will install all dependencies and create a new ``conda`` environment called ``wdtools``. Make sure to activate this environment before using wdtools. If you use Jupyter Notebooks, make sure the ``nb_conda`` package is installed to enable environment selection in Jupyter from the 'Kernel' menu.

In case you wish to load the wdtools dependencies into an existing environment (not recommended), first deactivate the environment and then run

.. code-block:: bash

   conda env update --name [your-environment] -f wdtools.yaml

This may cause version conflicts with existing packages in that environment, so we encourage you to use our first method. In case there are any problems with installation, please don't hesitate to contact the authors or raise a new issue on the GitHub page. 

Installing wdtools
++++++++++++++++++++

The simplest way to install wdtools is to clone the GitHub repository into your working directory:

.. code-block:: bash

   cd ~/
   git clone https://github.com/vedantchandra/wdtools.git

You can replace the first line with any working directory of your choice. It may be convenient to keep it in a high level directory to make it accesible to all your projects. Add the following lines to your Python projects to import wdtools into your workspace:

.. code-block:: python

   import sys
   sys.path.append('~/wdtools/')
   
   import wdtools

And you're done! 