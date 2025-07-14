

- MapKit JS
- Route
-  name 

Instance Property

# name

The name assigned to the route.

MapKit JS 5.0+

``` source
attribute string name;
```

## Discussion

Display name to the user so they can distinguish one route from another. MapKit JS localizes this string according to the mapkit.Directions object’s language value.

## See Also

### Route details

steps

An array of steps that compose the overall route.

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

