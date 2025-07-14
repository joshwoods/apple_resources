

- MapKit JS
- DirectionsRequest
-  origin 

Instance Property

# origin

The starting point for routing directions.

MapKit JS 5.0+

``` source
attribute string|mapkit.Coordinate|Place origin;
```

## Discussion

The `orgin` can be a string that’s an address, a coordinate, or a Place object.

## See Also

### Directions request

destination

The end point for routing directions.

arrivalDate

The arrival date for the trip.

departureDate

The departure date for the trip.

requestsAlternateRoutes

A Boolean value that indicates whether the server returns multiple routes when they’re available.

transportType

The mode of transportation the directions apply to.

avoidTolls

A Boolean value that prioritizes routes to avoid tolls.

mapkit.Directions.Transport

The modes of transportation.

