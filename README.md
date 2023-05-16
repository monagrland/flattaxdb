Parse and query different taxonomic databases
=============================================

Aims
----
* Work with taxonomic databases from data dump flatfiles.
* Load them directly into memory for queries and other operations.
* Use same internal data structures and methods for different source DBs.
* Report output as far as possible with DwC terms.

Such functionality is available with the R package
[`taxadb`](https://github.com/ropensci/taxadb), but we wish to work in Python
with few dependencies as possible.


Databases supported
-------------------
* NCBI Taxonomy (names.dmp and nodes.dmp file from taxdump)
* GBIF Backbone Taxonomy (Taxon.tsv file from backbone dump)
