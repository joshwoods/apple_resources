

- MapKit
- MKDirections
- MKDirections.ETAResponse
-  transportType 

Instance Property

# transportType

The type of conveyance to use for determining the travel time.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var transportType: MKDirectionsTransportType { get }
```

## Discussion

You specify the desired transportation type in your MKDirections.Request object. If you specified any, this property contains the transportation type used to generate the estimated information.

## See Also

### Getting the travel information

var expectedTravelTime: TimeInterval

The expected travel time, in seconds.

var expectedDepartureDate: Date

The expected departure time.

var expectedArrivalDate: Date

The expected arrival time.

var distance: CLLocationDistance

The expected travel distance, in meters.

