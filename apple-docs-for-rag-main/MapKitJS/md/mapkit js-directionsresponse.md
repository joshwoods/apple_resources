

- MapKit JS
-  DirectionsResponse 

Structure

# DirectionsResponse

The directions and estimated travel time that return for a route.

MapKit JS 5.0+

``` source
dictionary DirectionsResponse {
 DirectionsRequest request;
 mapkit.Coordinate?|Place? origin;
 mapkit.Coordinate?|Place? destination;
 Route[] routes;
};
```

## Mentioned in 

MapKit JS 5

## Overview

To get directions, create an instance of mapkit.Directions and call the route method.

When your code calls the route function, MapKit JS returns a `DirectionsResponse` asynchronously via a callback function. MapKit JS invokes the callback function with two arguments, `error` and `data` on failure and success. The `data` parameter is a `DirectionsResponse` object, and the `error` parameter contains an error code and text description of the error.

## Topics

### Directions response

request

The request object associated with the direction’s response.

routes

An array of route objects.

origin

An optional starting point for routing directions.

destination

An optional end point for routing directions.

## See Also

### Getting directions

route

Retrieves directions and estimated travel time based on the specified start and end points.

DirectionsRequest

The requested start and end points for a route, as well as the planned mode of transportation.

Route

Information about a route, including step-by-step instructions, distance, and estimated travel time.

RouteStep

A single step of the route between the requested start and end points.

