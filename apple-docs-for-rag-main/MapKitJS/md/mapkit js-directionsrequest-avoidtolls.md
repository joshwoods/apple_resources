

- MapKit JS
- DirectionsRequest
-  avoidTolls 

Instance Property

# avoidTolls

A Boolean value that prioritizes routes to avoid tolls.

MapKit JS 5.72+

``` source
attribute boolean? avoidTolls;
```

## Discussion

Set this value to `true` to prioritize routes that don’t have any tolls. The returned routes may contain tolls if no reasonable toll-free routes exist, even if `avoidTolls` is `true`. To verify toll assumptions, check hasTolls. The default is `false`.

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

transportType

The mode of transportation the directions apply to.

mapkit.Directions.Transport

The modes of transportation.

