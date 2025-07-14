

- MapKit JS
- DirectionsRequest
-  transportType 

Instance Property

# transportType

The mode of transportation the directions apply to.

MapKit JS 5.0+

``` source
attribute mapkit.Directions.Transport? transportType;
```

## Discussion

You can use this property to specify whether you want directions suited to a particular type of transportation. For example, you can specify if you want walking directions or driving directions.

The default value of this property is Automobile.

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

requestsAlternateRoutes

A Boolean value that indicates whether the server returns multiple routes when they’re available.

avoidTolls

A Boolean value that prioritizes routes to avoid tolls.

mapkit.Directions.Transport

The modes of transportation.

