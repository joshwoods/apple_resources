

- MapKit JS
- DirectionsRequest
-  departureDate 

Instance Property

# departureDate

The departure date for the trip.

MapKit JS 5.44+

``` source
attribute Date? departureDate;
```

## Mentioned in 

MapKit JS 5

## Discussion

Specify either a `departureDate` or an arrivalDate, don’t set both. If you send both values, MapKit JS logs a warning.

## See Also

### Directions request

origin

The starting point for routing directions.

destination

The end point for routing directions.

arrivalDate

The arrival date for the trip.

requestsAlternateRoutes

A Boolean value that indicates whether the server returns multiple routes when they’re available.

transportType

The mode of transportation the directions apply to.

avoidTolls

A Boolean value that prioritizes routes to avoid tolls.

mapkit.Directions.Transport

The modes of transportation.

