

- MapKit JS
-  RouteStep 

Structure

# RouteStep

A single step of the route between the requested start and end points.

MapKit JS 5.0+

``` source
dictionary RouteStep {
 mapkit.Coordinate[] path;
 string instructions;
 number distance;
 mapkit.Directions.Transport transportType;
};
```

## Overview

A RouteStep encapsulates information for a discrete segment of a route. A Route object’s steps property is an array of RouteStep objects. You don’t instantiate RouteStep objects directly; MapKit JS returns them as part of the DirectionsResponse.

## Topics

### Route step geometry

path

An array of coordinate objects representing the path of the route segment.

### Route step details

instructions

The written instructions for following the path that the step represents.

distance

The step distance, in meters.

transportType

The transport type of the step.

mapkit.Directions.Transport

The modes of transportation.

## See Also

### Getting directions

route

Retrieves directions and estimated travel time based on the specified start and end points.

DirectionsRequest

The requested start and end points for a route, as well as the planned mode of transportation.

DirectionsResponse

The directions and estimated travel time that return for a route.

Route

Information about a route, including step-by-step instructions, distance, and estimated travel time.

