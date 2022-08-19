Usage
=====

Note that Svetlana works with all kinds of image types (2D, 3D, multichannel).
A Youtube tutorial video is available here.

.. _annotation:

Annotation
------------

Organizing the data
~~~~~~~~~~~~~~~~~~~
First of all, you need your image(s) to be segmented in a certain way. Each ROI
of the segmentation mask must be given a unique integer value (label),
so each ROI can then be classified. To segment cells, you can refer to Cellpose for instance.

Once you segmented your data, it must be organized in a specific way:
::

    parent folder
    ├── Images
    │   ├── image1
    │   ...
    │   └── imageN
    ├── Masks
    │  ├── mask1
    │   ...
    │  └── maskN

The parent folder name doesn't matter, nevertheless the subfolder Images and Masks must
**absolutely** be called this way.

The labelling
~~~~~~~~~~~~~~~~~~~
Now the dataset is well organized, we can start annotating.

First, data must be loaded, loading the parent folder. Then, there are two ways to label,
whatever the type of image (2D, 3D etc).

#. Letting Svetlana propose patches one after another in a random order (default way).
#. Clicking on the objects, then clicking the label number. Can be useful in case the dataset is unbalanced in terms of cells number of each class in the image.

Saving the result
~~~~~~~~~~~~~~~~~~~
Once the user is satisfied by the number of ROI he made, he can click on
**save the result** button to create a binary file stored in a folder called
Svetlana.

This binary file called labels is then going to be used by the training plugin.

.. _training:
Training
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

.. _prediction:
Prediction
----------------

