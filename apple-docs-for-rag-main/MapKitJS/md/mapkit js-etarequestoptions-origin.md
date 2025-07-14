

- MapKit JS
- EtaRequestOptions
-  origin 

Instance Property

# origin

The starting point for estimated arrival time requests.

MapKit JS 5.46+

``` source
attribute mapkit.Coordinate origin;
```

## Discussion

The origin can be a mapkit.Coordinate, a Place object, or a string that’s an address. Other services, such as Search and Geocoder, return Place objects.

## See Also

### ETA Request

departureDate

The time of departure used in an estimated arrival time request.

destinations

An array of coordinates that represent end points for estimated arrival time requests.

transportType

The mode of transportation the server uses when estimating arrival times.

