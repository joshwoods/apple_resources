

- MapKit
- MKDirections
- MKDirections.ETAResponse
-  expectedArrivalDate 

Instance Property

# expectedArrivalDate

The expected arrival time.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var expectedArrivalDate: Date { get }
```

## Discussion

The value of this property is dependent on whether you specify a departure date or arrival date in your MKDirections.Request object. If you specify a departure date, the framework computes the date in this property by starting at your departure date and adding the expected travel time. If you specify an arrival time, but not a departure date, the framework sets this property to your arrival time. If you don’t specify an arrival date or departure date, the framework sets this property to the date that results by adding the travel time to the current time.

## See Also

### Getting the travel information

var expectedTravelTime: TimeInterval

The expected travel time, in seconds.

var expectedDepartureDate: Date

The expected departure time.

var distance: CLLocationDistance

The expected travel distance, in meters.

var transportType: MKDirectionsTransportType

The type of conveyance to use for determining the travel time.

