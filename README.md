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

Database files have to be separately downloaded. Links to zip archives of
versions that have been tested are below. Only the NCBI Taxonomy and GBIF
Backbone Taxonomy dump files are currently supported.

* NCBI Taxonomy (names.dmp and nodes.dmp file from taxdump)
  * Tested with version [2022-12-01](https://ftp.ncbi.nih.gov/pub/taxonomy/taxdump_archive/taxdmp_2022-12-01.zip)
* GBIF Backbone Taxonomy (Taxon.tsv file from backbone dump)
  * Tested with version [2021-11-26](https://hosted-datasets.gbif.org/datasets/backbone/2021-11-26/backbone.zip)


Installation and usage
----------------------

Install with pip

```bash
python3 -m pip install flattaxdb
```

Import and get help message in Python

```python
from flattaxdb import db
help(db.TaxonDB)
```
