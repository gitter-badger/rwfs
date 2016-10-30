## CHANGES IN VERSION 0.2.0 (2016-10-26)

### MAJOR CHANGES

+ `ogr2ogr` command-line conversion is not required anymore for
reading in data, even from WFS 2.0.0 source. It is still available
as an optional feature in `WFSCachingClient`. This change should
make it easier to use the package on various platforms where
`ogr2ogr` is not necessarily available or easy to set up.

### NEW FEATURES

+ Class `WFSStreamingRequest` has a new method `getParameters()`
for quering the request object's current parameters.

### OTHER

+ Basic tests using `testthat` in place.
+ Use `download.file(methods = "internal", mode = "wb")` in `ẀFSClient::getRaster()`.