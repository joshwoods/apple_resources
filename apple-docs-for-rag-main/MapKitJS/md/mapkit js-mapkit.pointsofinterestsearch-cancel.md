

- MapKit JS
- mapkit.PointsOfInterestSearch
-  cancel 

Instance Method

# cancel

Cancels a search request using its request ID.

MapKit JS 5.45+

``` source
boolean cancel(
 number id
);
```

## Parameters 

`id`  

Pass the integer ID returned by a call to search. The system ignores an invalid ID or the ID of a request that has completed.

## Return Value

`true` if the server canceled the pending search request.

## Discussion

Cancel an uncompleted search request by providing its request ID, the value returned from a call to search, to this method.

