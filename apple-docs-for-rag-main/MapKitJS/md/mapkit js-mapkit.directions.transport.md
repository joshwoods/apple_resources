

- MapKit JS
-  mapkit.Directions.Transport 

Enumeration

# mapkit.Directions.Transport

The modes of transportation.

MapKit JS 5.0+

``` source
interface mapkit.Directions.Transport {
 const string Automobile;
 const string Walking;
};
```

## Overview

Constants that describe the mode of transportation in DirectionsRequest and DirectionsResponse.

## Topics

### Transport types

Walking

A constant identifying the mode of transportation as walking.

Automobile

A constant identifying the mode of transportation as driving.

## See Also

### Directions request

origin

The starting point for routing directions.

destination

The end point for routing directions.

arrivalDate

The arrival date for the trip.

departureDate

The departure date for the trip.

requestsAlternateRoutes

A Boolean value that indicates whether the server returns multiple routes when they’re available.

transportType

The mode of transportation the directions apply to.

avoidTolls

A Boolean value that prioritizes routes to avoid tolls.

