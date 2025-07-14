

- MapKit
- MKLocalSearch
- MKLocalSearch.Request
-  region 

Instance Property

# region

A map region that provides a hint as to where to search.

iOS 6.1+iPadOS 6.1+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var region: MKCoordinateRegion { get set }
```

## Discussion

You can use this parameter to narrow the list of search results to those inside or close to the specified region. Specifying a region doesn’t ensure that the results are all inside the region. It’s merely a hint to the search engine.

## See Also

### Configuring the search parameters

var addressFilter: MKAddressFilter?

A filter that lists which address options to include or exclude in search results.

var naturalLanguageQuery: String?

A string containing the desired search item.

static var physicalFeature: MKLocalSearch.ResultType

A value that indicates that search results include physical features.

var pointOfInterestFilter: MKPointOfInterestFilter?

A filter that lists point-of-interest categories to include or exclude in search results.

var regionPriority: MKLocalSearchRegionPriority

A value that indicates the importance of the configured region.

var resultTypes: MKLocalSearch.ResultType

The types of items to include in the search results.

typealias ResultType

Options that indicate types of search results.

