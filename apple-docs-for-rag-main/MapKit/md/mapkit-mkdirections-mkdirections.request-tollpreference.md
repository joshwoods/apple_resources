

- MapKit
- MKDirections
- MKDirections.Request
-  tollPreference 

Instance Property

# tollPreference

The value that indicates whether the framework avoids routes that have tolls when providing directions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var tollPreference: MKDirections.RoutePreference { get set }
```

## See Also

### Specifying transportation options

var transportType: MKDirectionsTransportType

The type of conveyance that the directions apply to.

var highwayPreference: MKDirections.RoutePreference

The value that indicates whether the framework uses or avoids highways when providing directions.

enum RoutePreference

Options that modify how the framework selects routes when calculating directions.

var requestsAlternateRoutes: Bool

A Boolean value that indicates whether your app requests multiple routes when they’re available.

var departureDate: Date?

The departure date for the trip.

var arrivalDate: Date?

The arrival date for the trip.

