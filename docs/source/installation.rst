.. _installation:
Installation
=====

First, we advise you to create a conda environment in Python 3.9, in which you will run Napari:

.. code-block:: console

	conda create -n svetlana_env python=3.9
	conda activate svetlana_env
	conda install pip
	python -m pip install "napari[all]"==0.4.17

It is essential to install this particular version of Napari, as Svetlana is not compatible with later versions. Then, Svetlana can be installed either directly from Napari's plugin manager, or typing:

.. code-block:: console

   pip install napari_svetlana

WARNING:

If you have a CUDA compatible GPU on your computer, some computations may be accelerated
using the `CuPy package <https://cupy.dev/>`_. Unfortunately, CuPy needs CUDA toolkit to be installed. This library can only be installed via Conda while the plugin is a pip plugin, so it must be installed manually for the moment:

.. code-block:: console

    conda install cudatoolkit=11.5

Also note that the library `Cucim <https://pypi.org/project/cucim/>`_ that we use to improve these performances, computing morphological operations on GPU
is unfortunately only available for Linux systems. Hence, if you are a Windows user, this installation is not necessary.
