rebound-js
==========

An ElasticSearch ODM for Node.js. Use ElasticSearch as your primary document store...Elastic DB!

Goals
=====

To provide an Object->Document Mapper (ODM) for Elasticsearch, enabling quick, OOTB development of CRUD apps backed by Elasticsearch as a document store, while still providing easy access to advanced configuration and search features.

We're just beginning, but I'm incorporating many of the lessons learned from several years of using Elasticsearch as a primary data store, running the gamut of use cases from schema-less "shove-it-and-forget-it" scenarios to highly specialized search analyzers and aggregations across multiple indices and document types.

Roadmap
-------

This is a tentative roadmap. No specific version targets, but the order-of-implementation is mostly accurate.

* Connection Configuration Abstractions
* Rebound Model -> ES schema mappings
* Rebound Model CRUD
* Rebound Model Validation
* ES Result -> Rebound Model mapping
* Multi-Index, Per-Model
* Search Abstraction, with a particular focus on supporting cross-model, and cross-index searches
* Snapshot / Restore Facilities
* Migrations / Index-level Version Control
* Versioning / Document-level Version Control

Testing
-------

Tests are written as integrated, behavioral tests of the exposed API. Included Vagrantfile to stand-up a live Elasticsearch instance (1.5 as of 03/26/2015)

* vagrant up
* npm test
