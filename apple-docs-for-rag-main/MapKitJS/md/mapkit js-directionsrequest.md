

- MapKit JS
-  DirectionsRequest 

Structure

# DirectionsRequest

The requested start and end points for a route, as well as the planned mode of transportation.

MapKit JS 5.0+

``` source
dictionary DirectionsRequest {
 string|mapkit.Coordinate|Place origin;
 string|mapkit.Coordinate|Place destination;
 mapkit.Directions.Transport? transportType;
 boolean? requestsAlternateRoutes;
 Date? arrivalDate;
 Date? departureDate;
 boolean? avoidTolls;
};
```

## Overview

Provide a `DirectionsRequest` object to the route method to get directions between two points, as shown in the code listing that follows. Direction requests require origin and destination.

```
var myDirections = new mapkit.Directions();
myDirections.route({ 
  origin: "San Francisco, CA", 
  destination: "Oakland, CA", 
  transportType: mapkit.Directions.Transport.Automobile }, 
  function(error, data) { 
    // Results return asynchronously via this callback function, in `data`
  } 
);
```

## Topics

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

mapkit.Directions.Transport

The modes of transportation.

## See Also

### Getting directions

route

Retrieves directions and estimated travel time based on the specified start and end points.

DirectionsResponse

The directions and estimated travel time that return for a route.

Route

Information about a route, including step-by-step instructions, distance, and estimated travel time.

RouteStep

A single step of the route between the requested start and end points.

