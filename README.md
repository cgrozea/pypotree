-- this is a simple adaptation that should produce the correct URLs for JupyterHub instead of collab --

# PyPotree (potree for jupyter notebooks and colab)

Allows to insert potree cells into jupyter and colab notebooks

Gabriele Facciolo, CMLA 2019

[![Try it on Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1It3EbWy9W8Xf65ikP-_tpkVdJRmvwTQT)


# Installation and dependencies

The main source code repository for this project is https://github.com/cmla/pypotree
It is written in Python and contains Potree and PotreeConverter. It was tested with Python 3.5 and 3.6.

`pypotree` requires C and C++ developement tools.

`pypotree` can be installed with `pip`:

    pip install pypotree

# Usage

In Colab: 

     import pypotree 
     import numpy as np
     xyz = np.random.random((100000,3))
     cloudpath = pypotree.generate_cloud_for_display(xyz)
     pypotree.display_cloud_colab(cloudpath)


In a Jupyter notebook:

     import pypotree 
     import numpy as np
     xyz = np.random.random((100000,3))
     cloudpath = pypotree.generate_cloud_for_display(xyz)
     pypotree.display_cloud(cloudpath)
