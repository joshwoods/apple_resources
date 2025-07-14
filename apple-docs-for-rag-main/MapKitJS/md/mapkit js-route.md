

- MapKit JS
-  Route 

Structure

# Route

Information about a route, including step-by-step instructions, distance, and estimated travel time.

MapKit JS 5.0+

``` source
dictionary Route {
 mapkit.PolylineOverlay polyline;
 mapkit.Coordinate[][] path;
 RouteStep[] steps;
 string name;
 number distance;
 number expectedTravelTime;
 mapkit.Directions.Transport transportType;
 boolean? hasTolls;
};
```

## Overview

A Route object encapsulates the complete information for a route that the server returns, including geometry that you can use to draw a path and step-by-step text instructions. You don’t instantiate Route objects directly; MapKit JS returns them as part of the DirectionsResponse.

## Topics

### Route geometry

polyline

An instance of a polyline overlay that represents the path of a route.

path

An array of coordinate objects representing the path of the route.

Deprecated

### Route details

steps

An array of steps that compose the overall route.

name

The name assigned to the route.

distance

The route distance, in meters.

expectedTravelTime

The expected travel time, in seconds.

transportType

The overall route transport type.

hasTolls

A Boolean value that indicates whether a route has tolls.

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

RouteStep

A single step of the route between the requested start and end points.

