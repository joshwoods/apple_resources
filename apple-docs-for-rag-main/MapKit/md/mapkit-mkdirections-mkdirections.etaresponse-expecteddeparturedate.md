

- MapKit
- MKDirections
- MKDirections.ETAResponse
-  expectedDepartureDate 

Instance Property

# expectedDepartureDate

The expected departure time.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var expectedDepartureDate: Date { get }
```

## Discussion

The value of this property is dependent on whether you specify a departure date or arrival date in your MKDirections.Request object. If you specify a departure date, the framework copies that date to this property. If you specify an arrival date, but not a departure date, the framework computes the departure date by subtracting the expected travel time from your arrival date. If you don’t specify an arrival date or departure date, the framework sets this property to the current time.

## See Also

### Getting the travel information

var expectedTravelTime: TimeInterval

The expected travel time, in seconds.

var expectedArrivalDate: Date

The expected arrival time.

var distance: CLLocationDistance

The expected travel distance, in meters.

var transportType: MKDirectionsTransportType

The type of conveyance to use for determining the travel time.

