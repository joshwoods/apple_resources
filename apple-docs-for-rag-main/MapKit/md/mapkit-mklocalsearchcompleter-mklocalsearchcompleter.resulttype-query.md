

- MapKit
- MKLocalSearchCompleter
- MKLocalSearchCompleter.ResultType
-  query 

Type Property

# query

A value that indicates that the search completer includes query completions in the result.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
static var query: MKLocalSearchCompleter.ResultType { get }
```

## Discussion

For example, the search string `cof` yields a completion for *coffee*.

## See Also

### Type properties

static var address: MKLocalSearchCompleter.ResultType

A value that indicates that the search completer includes address completions in the result.

static var pointOfInterest: MKLocalSearchCompleter.ResultType

A value that indicates that the search completer includes point-of-interest completions in the result.

static var physicalFeature: MKLocalSearchCompleter.ResultType

A value that indicates that the search completer includes physical feature completions in the result.

