

- MapKit
- MKLocalSearch
- MKLocalSearch.Response
-  boundingRegion 

Instance Property

# boundingRegion

The map region that encloses the returned search results.

iOS 6.1+iPadOS 6.1+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var boundingRegion: MKCoordinateRegion { get }
```

## Discussion

The returned region is the smallest bounding box that encloses all of the map items. If there’s only one search result, the size of the region may be `(0, 0)`.

## See Also

### Getting the search results

var mapItems: [MKMapItem]

An array of map items representing the search results.

