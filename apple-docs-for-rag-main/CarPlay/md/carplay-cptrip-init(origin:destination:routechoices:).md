

- CarPlay
- CPTrip
-  init(origin:destination:routeChoices:) 

Initializer

# init(origin:destination:routeChoices:)

Creates a trip with an origin, destination, and route choices.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init(
    origin: MKMapItem,
    destination: MKMapItem,
    routeChoices: [CPRouteChoice]
)
```

## Parameters 

`origin`  

The trip’s origin.

`destination`  

The trip’s destination.

`routeChoices`  

Up to three route choices available for the trip.

## Return Value

A newly initialized trip.

## See Also

### Creating a Trip

class CPRouteChoice

A possible route for a trip.

