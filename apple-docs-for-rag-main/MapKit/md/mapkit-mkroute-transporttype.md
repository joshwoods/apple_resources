

- MapKit
- MKRoute
-  transportType 

Instance Property

# transportType

The overall route transport type.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var transportType: MKDirectionsTransportType { get }
```

## Discussion

This property reflects the primary transport type used for the route. Individual steps of the route might use different transport types.

## See Also

### Getting additional route details

var name: String

The assigned name for the route.

var hasHighways: Bool

A Boolean value that indicates whether the route contains highways.

var hasTolls: Bool

A Boolean value that indicates whether the route has tolls.

var advisoryNotices: [String]

An array of advisory notice strings for the route.

var distance: CLLocationDistance

The route distance, in meters.

var expectedTravelTime: TimeInterval

The expected travel time, in seconds.

