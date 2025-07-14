

- MapKit
- MKLocalSearchCompleter
-  filterType Deprecated

Instance Property

# filterType

The filter options for the search results.

iOS 9.3–13.0DeprecatediPadOS 9.3–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.11.4–10.15DeprecatedtvOS 9.2–13.0Deprecated

``` source
var filterType: MKLocalSearchCompleter.FilterType { get set }
```

Deprecated

Use resultTypes instead.

## Discussion

Use this property to determine whether you want completions that represent points-of-interest or whether completions might yield additional relevant query strings.

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

var resultTypes: MKLocalSearchCompleter.ResultType

The types of search completions to include.

var pointOfInterestFilter: MKPointOfInterestFilter?

A filter that lists point of interest categories to include or exclude in the search.

enum FilterType

Constants indicating the types of search completions to return.

Deprecated

struct ResultType

Options that indicate types of search completions.

