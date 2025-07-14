

- MapKit JS
- DirectionsRequest
-  requestsAlternateRoutes 

Instance Property

# requestsAlternateRoutes

A Boolean value that indicates whether the server returns multiple routes when they’re available.

MapKit JS 5.0+

``` source
attribute boolean? requestsAlternateRoutes;
```

## Discussion

When this property is `false`, the server returns a single route between the start and end points. When this property is `true`, the server may return additional routes for the user to follow. The server returns additional routes only if they’re available and represent a reasonable path that the user might take.

The default value of this property is `true`.

## See Also

### Directions request

origin

The starting point for routing directions.

destination

The end point for routing directions.

arrivalDate

The arrival date for the trip.

departureDate

The departure date for the trip.

transportType

The mode of transportation the directions apply to.

avoidTolls

A Boolean value that prioritizes routes to avoid tolls.

mapkit.Directions.Transport

The modes of transportation.

