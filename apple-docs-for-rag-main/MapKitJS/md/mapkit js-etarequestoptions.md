

- MapKit JS
-  EtaRequestOptions 

Structure

# EtaRequestOptions

The options you may provide for requesting estimated arrival times.

MapKit JS 5.46+

``` source
dictionary EtaRequestOptions {
 mapkit.Coordinate origin;
 mapkit.Coordinate[] destinations;
 mapkit.Directions.Transport transportType;
 Date departureDate;
};
```

## Overview

EtaRequestOptions accepts an array of destinations, but only accepts one `origin`, one `transportType`, and one `departureDate`. In other words, you can request the estimated arrival times from one place to 10 other places via one mode of transportation at one time.

## Topics

### ETA Request

origin

The starting point for estimated arrival time requests.

departureDate

The time of departure used in an estimated arrival time request.

destinations

An array of coordinates that represent end points for estimated arrival time requests.

transportType

The mode of transportation the server uses when estimating arrival times.

## See Also

### Getting estimated arrival times

eta

Retrieves estimated arrival times to up to 10 destinations from a single starting point.

EtaResponse

The estimated arrival times for a set of destinations.

EtaResult

The mode of transportation, distance, and travel time estimates for a single destination.

