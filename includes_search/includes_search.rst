.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

Search indexes allow queries to be made for any type of data that is indexed by the |chef server|, including data bags (and data bag items), environments, nodes, and roles. A defined query syntax is used to support search patterns like exact, wildcard, range, and fuzzy. A search is a full-text query that can be done from several locations, including from within a recipe, by using the ``search`` subcommand in |knife|, or by using the ``/search`` or ``/search/INDEX`` endpoints in the |api chef server|. The search engine is based on |apache solr| and is run from the |chef server|.

.. removing this: ", by using the search functionality in the |chef manage| add-on,"