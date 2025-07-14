

- MapKit
- MKDirections
- MKDirections.Request
-  arrivalDate 

Instance Property

# arrivalDate

The arrival date for the trip.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOSvisionOS 1.0+

``` source
var arrivalDate: Date? { get set }
```

## Discussion

Specifying an arrival date provides the server with extra information that it can use to optimize the returned routes. For example, for a trip that takes place during commute hours, the server might consider alternatives to routes that are typically congested at that time.

The use of this property is optional.

## See Also

### Specifying transportation options

var transportType: MKDirectionsTransportType

The type of conveyance that the directions apply to.

var highwayPreference: MKDirections.RoutePreference

The value that indicates whether the framework uses or avoids highways when providing directions.

var tollPreference: MKDirections.RoutePreference

The value that indicates whether the framework avoids routes that have tolls when providing directions.

enum RoutePreference

Options that modify how the framework selects routes when calculating directions.

var requestsAlternateRoutes: Bool

A Boolean value that indicates whether your app requests multiple routes when they’re available.

var departureDate: Date?

The departure date for the trip.

