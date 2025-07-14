

- MapKit JS
-  EtaResult 

Structure

# EtaResult

The mode of transportation, distance, and travel time estimates for a single destination.

MapKit JS 5.46+

``` source
dictionary EtaResult {
 mapkit.Directions.Transport transportType;
 mapkit.Coordinate destination;
 number distance;
 number expectedTravelTime;
 number staticTravelTime;
};
```

## Topics

### Estimated Arrival Times

transportType

The mode of transportation used to estimate the arrival time.

destination

The coordinates that represent the endpoint for estimated arrival time requests.

distance

The route distance in meters.

expectedTravelTime

The estimated travel time in seconds, including delays due to traffic.

staticTravelTime

The estimated travel time in seconds, excluding delays for traffic.

## See Also

### Getting estimated arrival times

eta

Retrieves estimated arrival times to up to 10 destinations from a single starting point.

EtaRequestOptions

The options you may provide for requesting estimated arrival times.

EtaResponse

The estimated arrival times for a set of destinations.

