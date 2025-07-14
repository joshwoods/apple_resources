

- MapKit
- MKLocalSearch
- MKLocalSearch.Response
-  mapItems 

Instance Property

# mapItems

An array of map items representing the search results.

iOS 6.1+iPadOS 6.1+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var mapItems: [MKMapItem] { get }
```

## Discussion

This property contains an array of MKMapItem objects, each of which represents a returned search result. You can use these objects to retrieve information about the search result, such as the name of the point of interest, the address, the geographic location, and so on.

## See Also

### Related Documentation

Location and Maps Programming Guide

### Getting the search results

var boundingRegion: MKCoordinateRegion

The map region that encloses the returned search results.

