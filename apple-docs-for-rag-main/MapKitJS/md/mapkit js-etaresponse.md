

- MapKit JS
-  EtaResponse 

Structure

# EtaResponse

The estimated arrival times for a set of destinations.

MapKit JS 5.46+

``` source
dictionary EtaResponse {
 Object request;
 mapkit.Coordinate origin;
 EtaResult[] etas;
};
```

## Topics

### Estimated Arrival Time Responses

request

The request object associated with the estimated time of arrival response.

origin

The coordinates that represent the starting point for estimated arrival time requests.

etas

An array of estimated arrival times.

## See Also

### Getting estimated arrival times

eta

Retrieves estimated arrival times to up to 10 destinations from a single starting point.

EtaRequestOptions

The options you may provide for requesting estimated arrival times.

EtaResult

The mode of transportation, distance, and travel time estimates for a single destination.

