

- MapKit JS
- mapkit.PointsOfInterestSearch
-  search 

Instance Method

# search

Fetches points of interest.

MapKit JS 5.45+

``` source
number search(
 function|PointsOfInterestSearchDelegate callback,
 optional PointsOfInterestSearchOptions options
);
```

## Parameters 

`callback`  

A callback function or delegate object with the following parameters:

`error` (Error)  
An error code and descriptive message.

`data` (PointsOfInterestSearchResponse)  
An object parsed from server-returned JSON.

`options`  

A PointsOfInterestSearchOptions object.

## Return Value

This method returns a request ID (integer) that you can use with cancel to abort a pending request.

## Discussion

The search method returns a set of points of interest within the region defined and matching the mapkit.PointOfInterestFilter.

MapKit JS invokes the `callback` function on failure and success with two arguments, `error` and `data` that represent failure and success information, respectively. You may optionally provide a delegate object instead of a callback. If you call cancel before MapKit JS responds, the callback or delegate isn’t called.

## See Also

### Fetching points of interest

PointsOfInterestSearchDelegate

An object or callback function that MapKit JS calls when fetching points of interest.

PointsOfInterestSearchResponse

The result of a request used to fetch points of interest.

