

- MapKit JS
- Route
-  steps 

Instance Property

# steps

An array of steps that compose the overall route.

MapKit JS 5.0+

``` source
attribute RouteStep[] steps;
```

## Discussion

The array contains one or more RouteStep objects representing distinct portions of the route. Each step corresponds to a single direction to follow along the route.

## See Also

### Route details

name

The name assigned to the route.

distance

The route distance, in meters.

expectedTravelTime

The expected travel time, in seconds.

transportType

The overall route transport type.

hasTolls

A Boolean value that indicates whether a route has tolls.

mapkit.Directions.Transport

The modes of transportation.

