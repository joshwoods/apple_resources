

- MapKit JS
- Route
-  distance 

Instance Property

# distance

The route distance, in meters.

MapKit JS 5.0+

``` source
attribute number distance;
```

## Discussion

This property reflects the distance that the user covers while traversing the path of the route. It isn’t a straight line distance between the origin and destination.

## See Also

### Route details

steps

An array of steps that compose the overall route.

name

The name assigned to the route.

expectedTravelTime

The expected travel time, in seconds.

transportType

The overall route transport type.

hasTolls

A Boolean value that indicates whether a route has tolls.

mapkit.Directions.Transport

The modes of transportation.

