

- MapKit JS
- Route
-  transportType 

Instance Property

# transportType

The overall route transport type.

MapKit JS 5.0+

``` source
attribute mapkit.Directions.Transport transportType;
```

## Discussion

This property reflects the primary transport type used for the route. Individual steps of the route might use different transport types.

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

hasTolls

A Boolean value that indicates whether a route has tolls.

mapkit.Directions.Transport

The modes of transportation.

