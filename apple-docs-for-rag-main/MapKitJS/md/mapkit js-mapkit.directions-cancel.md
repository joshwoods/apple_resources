

- MapKit JS
- mapkit.Directions
-  cancel 

Instance Method

# cancel

Cancels a previous request for routes or estimated arrival times.

MapKit JS 5.0+

``` source
boolean cancel(
 number id
);
```

## Parameters 

`id`  

The ID that returns from a call to route or eta. Passing an invalid ID or the ID of a completed request has no effect.

## Return Value

cancel returns `true` if the server cancels the pending route or eta request. cancel returns `false` if the server can’t cancel the route or eta request.

## Discussion

Sometimes you need to cancel a request, either because the user initiates the cancellation or moves on to another activity. You can cancel a route or eta request by providing its ID.

