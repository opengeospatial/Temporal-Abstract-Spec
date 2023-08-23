# Abstract Specification on Time

This repo is for the OGC Temporal Domain Working Group to develop an Abstract Specification for Time to be part of the [Abstract Specifications](https://www.ogc.org/docs/as), described in more detail in [OGC Abstract Specification Topic 0](https://docs.ogc.org/as/04-084r4/04-084r4.html) 

The current OGC standards generally refer to the ISO documents such as [ISO 19108](https://www.iso.org/standard/26013.html), and their freely available OGC equivalents, such as [Abstract Specification Topic 2 Referencing by Coordinates](https://docs.opengeospatial.org/as/18-005r4/18-005r4.html#44).

Much effort over decades has gone into establishing complex structures to represent calendar based time, such as the ISO8601 notation, and many date-time schemas. Because of this effort, many people use calendar based "coordinates", with the attendant ambiguities, imprecision and inappropriate scope.

The aim of the document is to establish a clear terminology, so that people are clearly aware of the advantages and disadvantages of adopting a particular technological approach and then perhaps help build better interoperable systems.

The current draft documents available from the following locations:

* Charter (draft) in [HTML](https://htmlpreview.github.io/?https://github.com/opengeospatial/Temporal-Abstract-Spec/blob/master/Charter/document.html), [PDF](https://github.com/opengeospatial/Temporal-Abstract-Spec/blob/master/Charter/document.pdf), and [Word](https://github.com/opengeospatial/Temporal-Abstract-Spec/blob/master/Charter/document.doc) formats.
* Abstract Specification (draft) in [HTML](https://htmlpreview.github.io/?https://github.com/opengeospatial/Temporal-Abstract-Spec/blob/master/23-049/23-049.html), [PDF](https://github.com/opengeospatial/Temporal-Abstract-Spec/blob/master/23-049/23-049.pdf), and [Word](https://github.com/opengeospatial/Temporal-Abstract-Spec/blob/master/23-049/23-049.doc) formats.

## About this document

Instructions on authoring OGC documents using the metanorma toolchain can be found at https://www.metanorma.org/author/ogc/authoring/

If there are any issues or problems with the toolchain, please raise them at https://github.com/metanorma/metanorma-ogc/issues

Copy in OGC staff by adding @ghobona to the Issue's body.

## To compile the document using a docker image

`docker run -v "$(pwd)":/metanorma -v ${HOME}/.fontist/fonts/:/config/fonts  metanorma/mn  metanorma compile --agree-to-terms -t ogc -x xml,html,doc,pdf document.adoc`

NOTE: You need to add the --agree-to-terms option to retrieve licenced fonts.

NOTE: This command caches fonts on your local system.

## Alternative approach for compilation

It is also possible to install the metanorma toolchain locally and to compile the document using the local instance of metanorma.
