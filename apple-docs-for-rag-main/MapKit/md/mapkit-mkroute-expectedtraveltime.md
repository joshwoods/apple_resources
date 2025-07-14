

- MapKit
- MKRoute
-  expectedTravelTime 

Instance Property

# expectedTravelTime

The expected travel time, in seconds.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var expectedTravelTime: TimeInterval { get }
```

## Discussion

This expected travel time reflects the time it takes to traverse the route under ideal conditions. The actual amount of time may vary based on conditions.

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

var transportType: MKDirectionsTransportType

The overall route transport type.

