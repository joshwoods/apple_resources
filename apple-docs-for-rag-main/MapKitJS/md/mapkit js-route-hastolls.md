

- MapKit JS
- Route
-  hasTolls 

Instance Property

# hasTolls

A Boolean value that indicates whether a route has tolls.

MapKit JS 5.72+

``` source
attribute boolean? hasTolls;
```

## Discussion

When `true`, this route has tolls. If `false`, this route doesn’t have any tolls. If undefined, the route may or may not have tolls.

## See Also

### Route details

steps

An array of steps that compose the overall route.

name

The name assigned to the route.

distance

The route distance, in meters.

expectedTravelTime

The expected travel time, in seconds.

transportType

The overall route transport type.

mapkit.Directions.Transport

The modes of transportation.

