

- MapKit
- MKLocalSearchCompleter
-  resultTypes 

Instance Property

# resultTypes

The types of search completions to include.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var resultTypes: MKLocalSearchCompleter.ResultType { get set }
```

## See Also

### Specifying the query attributes

var addressFilter: MKAddressFilter?

A filter that lists which address options to include or exclude in search results.

var queryFragment: String

The search string that you want completions for.

var region: MKCoordinateRegion

The region that defines the geographic scope of the search.

var regionPriority: MKLocalSearchRegionPriority

A value that indicates the importance of the configured region.

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

