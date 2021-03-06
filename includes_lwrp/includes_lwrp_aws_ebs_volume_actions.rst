.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

This lightweight resource provider has the following actions:

.. list-table::
   :widths: 200 300
   :header-rows: 1

   * - Action
     - Description
   * - ``:attach``
     - Use to attach an existing volume to a node.
   * - ``:create``
     - Use to create a new |amazon ebs| volume. This action will only make the API call to create a new volume, which will get a random volume identifier that is generated by |amazon ec2|. This identifier can be attached in the same resource by specifying the actions as an array.
   * - ``:detach``
     - Use to detach the specified volume from a node.
   * - ``:prune``
     - Use to prune older snapshots from a node.
   * - ``:snapshot``
     - Use to create a snapshot of the volume.

