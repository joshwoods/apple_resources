

- MapKit
- MKDirections
- MKDirections.Request
-  transportType 

Instance Property

# transportType

The type of conveyance that the directions apply to.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOSvisionOS 1.0+

``` source
var transportType: MKDirectionsTransportType { get set }
```

## Discussion

You can use this property to specify whether you want directions suited to a particular type of transportation. For example, you can use this to specify that you want walking directions or driving directions.

The default value of this property is any.

## See Also

### Specifying transportation options

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

var arrivalDate: Date?

The arrival date for the trip.

