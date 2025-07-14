

- MapKit
- MKLocalSearchCompleter
- MKLocalSearchCompleter.ResultType
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a direction transport type using a raw unsigned integer value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
init(rawValue: UInt)
```

## Parameters 

`rawValue`  

The unsigned integer value of the direction transport type.

## See Also

### Initializers

static var address: MKLocalSearchCompleter.ResultType

A value that indicates that the search completer includes address completions in the result.

static var pointOfInterest: MKLocalSearchCompleter.ResultType

A value that indicates that the search completer includes point-of-interest completions in the result.

static var physicalFeature: MKLocalSearchCompleter.ResultType

A value that indicates that the search completer includes physical feature completions in the result.

static var query: MKLocalSearchCompleter.ResultType

A value that indicates that the search completer includes query completions in the result.

