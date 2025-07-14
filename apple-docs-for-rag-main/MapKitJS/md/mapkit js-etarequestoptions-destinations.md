

- MapKit JS
- EtaRequestOptions
-  destinations 

Instance Property

# destinations

An array of coordinates that represent end points for estimated arrival time requests.

MapKit JS 5.46+

``` source
attribute mapkit.Coordinate[] destinations;
```

## Discussion

A mapkit.Coordinate represents each destination in the array. You may get coordinates from search or lookup, which return Place objects that contain coordinates. You may provide up to 10 destinations in the array.

## See Also

### ETA Request

origin

The starting point for estimated arrival time requests.

departureDate

The time of departure used in an estimated arrival time request.

transportType

The mode of transportation the server uses when estimating arrival times.

