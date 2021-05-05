# Abstract Specification on Time

## About this document



Instructions on authoring OGC documents using the metanorma toolchain can be found at https://www.metanorma.org/author/ogc/authoring/

If there are any issues or problems with the toolchain, please raise them at https://github.com/metanorma/metanorma-ogc/issues

Copy in OGC staff by adding @ghobona to the Issue's body.

## To compile the document using a docker image

`docker run -v "$(pwd)":/metanorma -v ${HOME}/.fontist/fonts/:/config/fonts  metanorma/mn  metanorma compile --agree-to-terms -t ogc -x xml,html,doc document.adoc`

NOTE: You need to add the --agree-to-terms option to retrieve licenced fonts.

NOTE: This command caches fonts on your local system.

## Alternative approach for compilation

It is also possible to install the metanorma toolchain locally and to compile the document using the local instance of metanorma.
