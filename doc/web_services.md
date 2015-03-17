# Introduction

The base URI for the web service is: `/ontobrowser/ontologies`

# Authentication


* `application/rdf+xml`
* `application/obo`

Note 1: There is no internet media type registered for the OBO format so the `text/obo` and `application/obo` media types are specific to the OntoBrowser web service.
 


# Example
The following example downloads the [Mouse adult gross anatomy](http://www.obofoundry.org/cgi-bin/detail.cgi?id=adult_mouse_anatomy) ontology then loads it into OntoBrowser using the web service:

```bash
$ curl -s -S -O -L http://purl.obolibrary.org/obo/ma.obo
$ curl -s -S -H "Content-Type: application/obo;charset=utf-8" -X PUT --data-binary "@ma.obo" -u SYSTEM "http://localhost/ontobrowser/ontologies/Mouse%20adult%20gross%20anatomy"
```