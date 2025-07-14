

- MapKit JS
- EtaResponse
-  etas 

Instance Property

# etas

An array of estimated arrival times.

MapKit JS 5.46+

``` source
attribute EtaResult[] etas;
```

## Discussion

The server returns etas as a part of the EtaResponse after your app creates an instance of the mapkit.Directions object and calls the eta method.

## See Also

### Estimated Arrival Time Responses

request

The request object associated with the estimated time of arrival response.

origin

The coordinates that represent the starting point for estimated arrival time requests.

