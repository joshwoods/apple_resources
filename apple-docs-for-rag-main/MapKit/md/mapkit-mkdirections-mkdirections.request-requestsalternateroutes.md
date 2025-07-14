

- MapKit
- MKDirections
- MKDirections.Request
-  requestsAlternateRoutes 

Instance Property

# requestsAlternateRoutes

A Boolean value that indicates whether your app requests multiple routes when they’re available.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOSvisionOS 1.0+

``` source
var requestsAlternateRoutes: Bool { get set }
```

## Discussion

When this property is false, the server returns a single route between the start and end points. When this property is true, the server may return additional routes for the user to follow. The server returns additional routes only if they’re available and represent a reasonable path that the user might take.

The default value of this property is false.

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

var departureDate: Date?

The departure date for the trip.

var arrivalDate: Date?

The arrival date for the trip.

