.. _installation:
Installation
=====

First, we advise you to create a conda environment in Python 3.9, in which you will run Napari:

.. code-block:: console

	conda create -n svetlana_env python=3.9
	conda activate svetlana_env
	conda install pip
	python -m pip install "napari[all]" --upgrade

Then, Svetlana can be installed either directly from Napari's plugin manager, or typing:

.. code-block:: console

   pip install napari_svetlana

WARNING:

If you have a CUDA compatible GPU on your computer, some computations may be accelerated
using the `CuPy package <https://cupy.dev/>`_. Unfortunately, CuPy needs CUDA toolkit to be installed. This library can only be installed via Conda while the plugin is a pip plugin, so it must be installed manually for the moment:

.. code-block:: console

    conda install cudatoolkit=10.2
