Welcome to Svetlana's documentation!
===================================

`Svetlana <https://www.napari-hub.org/plugins/napari-svetlana>`_ is a Napari plugin developed in Python, dedicated to the classification of segmentation masks.
It has mainly been developed for biological imaging, but it can be applied to any kind of 2D, 3D or multichannel
segmented image.

The classifier is based on light-weight convolutional neural networks and is efficient with few annotations. You can
learn more about our method reading the `related paper <https://hal.inria.fr/hal-03927879>`_.

First check out the :doc:`installation` section to know how to install it.

A Youtube tutorial video is available `here <https://www.youtube.com/watch?v=u_FKuHta-RE>`_. You can also have a look at :doc:`usage` to know more about advanced
features. **Two demo images**, similar to the ones of the tutorial video, are available in the
`git repository <https://bitbucket.org/koopa31/napari_svetlana/src/main/>`_, so you can easily
reproduce it, and test the features by yourself.

If you use this plugin, please cite the paper:

.. code-block:: bibtex

    @unpublished{weiss:hal-03927879,
      TITLE = {{Svetlana: a Supervised Segmentation Classifier for Napari}},
      AUTHOR = {Weiss, Pierre and Cazorla, Cl{\'e}ment and Morin, Renaud},
      URL = {https://hal.inria.fr/hal-03927879},
      NOTE = {working paper or preprint},
      YEAR = {2023},
      MONTH = Jan,
      PDF = {https://hal.inria.fr/hal-03927879/file/main_nature.pdf},
      HAL_ID = {hal-03927879},
      HAL_VERSION = {v1},
    }


.. note::

   This project is still under active development. We welcome any suggestions for improvement from users.
    Thank you

.. figure:: https://raw.githubusercontent.com/koopa31/Svetlana_documentation/main/docs/images/napari.png
    :width: 100 %


Contents
--------

.. toctree::
   installation
   usage
