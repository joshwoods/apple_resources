

- MapKit
- MKDirections
- MKDirections.ETAResponse
-  expectedTravelTime 

Instance Property

# expectedTravelTime

The expected travel time, in seconds.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var expectedTravelTime: TimeInterval { get }
```

## Discussion

The expected travel time reflects the time it takes to traverse the route, taking expected traffic into account. The actual amount of time may vary based on changes in traffic and other travel conditions.

## See Also

### Getting the travel information

var expectedDepartureDate: Date

The expected departure time.

var expectedArrivalDate: Date

The expected arrival time.

var distance: CLLocationDistance

The expected travel distance, in meters.

var transportType: MKDirectionsTransportType

The type of conveyance to use for determining the travel time.

