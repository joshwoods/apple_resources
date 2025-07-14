

- MapKit
- MKLocalSearchCompleter
-  MKLocalSearchCompleter.FilterType Deprecated

Enumeration

# MKLocalSearchCompleter.FilterType

Constants indicating the types of search completions to return.

iOS 9.3–13.0DeprecatediPadOS 9.3–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.11.4–10.15DeprecatedtvOS 9.2–13.0Deprecated

``` source
enum FilterType
```

Deprecated

Use MKLocalSearchCompleter.ResultType instead.

## Topics

### Constants

case locationsAndQueries

Points of interest and query suggestions. Specify this value when you want both map-based points of interest and common query terms used to find locations. For example, the search string `cof` yields a completion for *coffee*.

case locationsOnly

Points of interest only. Specify this value when you want the search string to yield completions that correspond to a specific point-of-interest on the map.

case locationsAndQueries

Points of interest and query suggestions. Specify this value when you want both map-based points of interest and common query terms used to find locations. For example, the search string `cof` yields a completion for *coffee*.

case locationsOnly

Points of interest only. Specify this value when you want the search string to yield completions that correspond to a specific point-of-interest on the map.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var filterType: MKLocalSearchCompleter.FilterType

The filter options for the search results.

Deprecated

struct ResultType

Options that indicate types of search completions.

