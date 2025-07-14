

- MapKit JS
- mapkit.Geocoder
-  cancel 

Instance Method

# cancel

Cancels the pending lookup or reverse lookup using its request ID.

MapKit JS 5.0+

``` source
boolean cancel(
 number id
);
```

## Parameters 

`id`  

The request ID of the lookup or reverseLookup to cancel.

## Return Value

Returns `true` if the system cancels a pending request.

## Discussion

Returns `false` if the request is already complete or if the request ID is invalid.

## Discussion

Sometimes you need to cancel a request, either because the user initiates the cancellation or moves on to another activity.

Cancel a geocoding lookup or reverseLookup by specifying its request ID, which MapKit JS returns when making the initial request.

