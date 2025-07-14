

- MapKit JS
- mapkit.Directions
-  route 

Instance Method

# route

Retrieves directions and estimated travel time based on the specified start and end points.

MapKit JS 5.0+

``` source
number route(
 DirectionsRequest request,
 function callback
);
```

## Parameters 

`request`  

A DirectionsRequest object that specifies details for the directions you want to retrieve.

`callback`  

A callback function that receives the directions, returned asynchronously.

## Return Value

A request ID, which you can pass to cancel to abort a pending request.

## Discussion

Call the route method to get directions.

MapKit JS returns directions asynchronously via a callback function. This callback function is invoked with two arguments, `error` on failure and `data` on success.

`error` contains an error code and a text description of the error. `data` is a DirectionsResponse object with the following two properties:

- `request` is the request object associated with this response.

- `routes` contains an array of up to three Route objects returned by the server.

## See Also

### Getting directions

DirectionsRequest

The requested start and end points for a route, as well as the planned mode of transportation.

DirectionsResponse

The directions and estimated travel time that return for a route.

Route

Information about a route, including step-by-step instructions, distance, and estimated travel time.

RouteStep

A single step of the route between the requested start and end points.

