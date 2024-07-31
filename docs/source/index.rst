Welcome to Svetlana's documentation!
===================================

`Svetlana <https://www.napari-hub.org/plugins/napari-svetlana>`_ is a Napari plugin developed in Python, dedicated to the classification of segmentation masks.
It has mainly been developed for biological imaging, but it can be applied to any kind of 2D, 3D or multichannel
segmented image.

The classifier is based on light-weight convolutional neural networks and is efficient with few annotations. You can
learn more about our method reading the `related paper <https://www.nature.com/articles/s41598-024-60916-8>`_.

First check out the :doc:`installation` section to know how to install it.

A Youtube tutorial video is available `here <https://www.youtube.com/watch?v=u_FKuHta-RE>`_. You can also have a look at :doc:`usage` to know more about advanced
features. **Two demo images**, identical to the ones of the tutorial video, are available in the annotation plugin using
the button **TRY ON DEMO IMAGE**. Feel free to use them to familiarize yourself with the plugin.

If you use this plugin, please cite the paper:

Cazorla, C., Weiss, P., & Morin, R. (2024). Svetlana a Supervised Segmentation Classifier for Napari.

.. code-block:: bibtex

    @article{cazorla2024svetlana,
      title={Svetlana a supervised segmentation classifier for Napari},
      author={Cazorla, Cl{\'e}ment and Morin, Renaud and Weiss, Pierre},
      journal={Scientific Reports},
      volume={14},
      number={1},
      pages={11604},
      year={2024},
      publisher={Nature Publishing Group UK London}
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
