

- MapKit JS
- EtaRequestOptions
-  departureDate 

Instance Property

# departureDate

The time of departure used in an estimated arrival time request.

MapKit JS 5.46+

``` source
attribute Date departureDate;
```

## Discussion

If you don’t specify a departure date, the server will use the current date and time when you make the request.

## See Also

### ETA Request

origin

The starting point for estimated arrival time requests.

destinations

An array of coordinates that represent end points for estimated arrival time requests.

transportType

The mode of transportation the server uses when estimating arrival times.

