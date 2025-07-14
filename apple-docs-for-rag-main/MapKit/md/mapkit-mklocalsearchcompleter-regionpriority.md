

- MapKit
- MKLocalSearchCompleter
-  regionPriority 

Instance Property

# regionPriority

A value that indicates the importance of the configured region.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var regionPriority: MKLocalSearchRegionPriority { get set }
```

## See Also

### Specifying the query attributes

var addressFilter: MKAddressFilter?

A filter that lists which address options to include or exclude in search results.

var queryFragment: String

The search string that you want completions for.

var region: MKCoordinateRegion

The region that defines the geographic scope of the search.

var resultTypes: MKLocalSearchCompleter.ResultType

The types of search completions to include.

var pointOfInterestFilter: MKPointOfInterestFilter?

A filter that lists point of interest categories to include or exclude in the search.

var filterType: MKLocalSearchCompleter.FilterType

The filter options for the search results.

Deprecated

enum FilterType

Constants indicating the types of search completions to return.

Deprecated

struct ResultType

Options that indicate types of search completions.

