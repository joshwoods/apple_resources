

- MapKit
- MKDirections
- MKDirections.ETAResponse
-  distance 

Instance Property

# distance

The expected travel distance, in meters.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var distance: CLLocationDistance { get }
```

## Discussion

This property contains the overall distance traversed by the route.

## See Also

### Getting the travel information

var expectedTravelTime: TimeInterval

The expected travel time, in seconds.

var expectedDepartureDate: Date

The expected departure time.

var expectedArrivalDate: Date

The expected arrival time.

var transportType: MKDirectionsTransportType

The type of conveyance to use for determining the travel time.

