

- MapKit
- MKLocalSearch
- MKLocalSearch.Request
-  MKLocalSearch.Request.ResultType 

Type Alias

# MKLocalSearch.Request.ResultType

Options that indicate types of search results.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS

``` source
typealias ResultType = MKLocalSearch.ResultType
```

## See Also

### Configuring the search parameters

var addressFilter: MKAddressFilter?

A filter that lists which address options to include or exclude in search results.

var naturalLanguageQuery: String?

A string containing the desired search item.

var region: MKCoordinateRegion

A map region that provides a hint as to where to search.

static var physicalFeature: MKLocalSearch.ResultType

A value that indicates that search results include physical features.

var pointOfInterestFilter: MKPointOfInterestFilter?

A filter that lists point-of-interest categories to include or exclude in search results.

var regionPriority: MKLocalSearchRegionPriority

A value that indicates the importance of the configured region.

var resultTypes: MKLocalSearch.ResultType

The types of items to include in the search results.

