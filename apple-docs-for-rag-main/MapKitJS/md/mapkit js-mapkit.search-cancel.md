

- MapKit JS
- mapkit.Search
-  cancel 

Instance Method

# cancel

Cancels a search request using its request ID.

MapKit JS 5.0+

``` source
boolean cancel(
 number id
);
```

## Parameters 

`id`  

Pass the integer ID that returns from a call to mapkit.Search. Passing an invalid ID or the ID of a completed request has no effect.

## Return Value

`true` if the server cancels the pending search request.

## Discussion

Sometimes you need to cancel a request, either because the user initiates the cancellation or moves on to another activity. Cancel a search request by providing its request ID, which MapKit JS returns from a call to search.

