

- MapKit JS
-  mapkit.Directions 

Class

# mapkit.Directions

An object that provides directions and estimated travel time based on the options you provide.

MapKit JS 5.0+

``` source
interface mapkit.Directions
```

## Mentioned in 

MapKit JS 5

## Topics

### Creating a directions object

mapkit.Directions

Creates a directions object with options you provide.

DirectionsConstructorOptions

Options that you may provide when creating a directions object.

### Getting estimated arrival times

eta

Retrieves estimated arrival times to up to 10 destinations from a single starting point.

EtaRequestOptions

The options you may provide for requesting estimated arrival times.

EtaResponse

The estimated arrival times for a set of destinations.

EtaResult

The mode of transportation, distance, and travel time estimates for a single destination.

### Getting directions

route

Retrieves directions and estimated travel time based on the specified start and end points.

DirectionsRequest

The requested start and end points for a route, as well as the planned mode of transportation.

DirectionsResponse

The directions and estimated travel time that return for a route.

Route

Information about a route, including step-by-step instructions, distance, and estimated travel time.

RouteStep

A single step of the route between the requested start and end points.

### Canceling a directions request

cancel

Cancels a previous request for routes or estimated arrival times.

