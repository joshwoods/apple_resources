

- MapKit
- MKLocalSearch
- MKLocalSearch.Request
-  regionPriority 

Instance Property

# regionPriority

A value that indicates the importance of the configured region.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var regionPriority: MKLocalSearchRegionPriority { get set }
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

var resultTypes: MKLocalSearch.ResultType

The types of items to include in the search results.

typealias ResultType

Options that indicate types of search results.

