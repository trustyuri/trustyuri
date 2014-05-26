![Trusty URI logo](logo/trustyuri.png)


Trusty URIs
===========


Here you find general information and documents about the trusty URI approach.


Important Documents
-------------------

The [trusty URI specification](https://github.com/trustyuri/trustyuri-spec)
formally defines the structure and meaning of trusty URIs.

The following article introduces the trusty URI approach:

> Tobias Kuhn and Michel Dumontier. Trusty URIs: Verifiable, Immutable, and
> Permanent Digital Artifacts for Linked Data. In _Proceedings of the 11th
> Extended Semantic Web Conference (ESWC)_. Springer, 2014.
> http://arxiv.org/abs/1401.5775

Check out the [wiki](https://github.com/trustyuri/trustyuri/wiki) for posting
your wish-list features, giving feedback, brainstorming, etc.


Example
-------

Generally, trusty URIs are URIs that contain a certain kind of hash value that
can be used to verify the respective resource. This is an example of a
trusty URI:

    http://example.org/r1.RAcbjcRIQozo2wBMq4WcCYkFAjRz0AX-Ux3PquZZrC68s

The last 45 characters of this URI (everything that comes after `r1.`) are the
artifact code of the trusty URI. The first two characters of the artifact code
(`RA` in this example) define the type and version of the module. (Only `FA`
for plain file content and `RA` for sets of RDF graphs are supported at this
point.) The remaining 43 characters are the actual hash value. This hash can
be used to check the content of the resource this URI represents.


Implementations
---------------

There are currently three (partial) implementations:

- trustyuri-java: https://github.com/trustyuri/trustyuri-java
- trustyuri-perl: https://github.com/trustyuri/trustyuri-perl
- trustyuri-python: https://github.com/trustyuri/trustyuri-python

