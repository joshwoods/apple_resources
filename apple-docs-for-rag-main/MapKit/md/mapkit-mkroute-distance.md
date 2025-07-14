

- MapKit
- MKRoute
-  distance 

Instance Property

# distance

The route distance, in meters.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var distance: CLLocationDistance { get }
```

## Discussion

This property reflects the distance that the user covers while traversing the path of the route. It’s not a linear distance between the start and end points of the route.

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

var expectedTravelTime: TimeInterval

The expected travel time, in seconds.

var transportType: MKDirectionsTransportType

The overall route transport type.

