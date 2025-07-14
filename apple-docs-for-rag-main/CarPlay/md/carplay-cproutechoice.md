

- CarPlay
-  CPRouteChoice 

Class

# CPRouteChoice

A possible route for a trip.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPRouteChoice
```

## Topics

### Creating a Route Choice

init(summaryVariants: [String], additionalInformationVariants: [String], selectionSummaryVariants: [String])

Creates a route choice.

### Getting Variants

var summaryVariants: [String]

An array of summary variants.

var additionalInformationVariants: [String]?

An array of variants providing additional information about the route choice.

var selectionSummaryVariants: [String]?

An array of selection summary variants.

### Providing Additional Information

var userInfo: Any?

An object containing custom information associated with the route choice.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Creating a Trip

init(origin: MKMapItem, destination: MKMapItem, routeChoices: [CPRouteChoice])

Creates a trip with an origin, destination, and route choices.

