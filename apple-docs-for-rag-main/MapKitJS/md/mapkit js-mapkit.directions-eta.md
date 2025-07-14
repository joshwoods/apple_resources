

- MapKit JS
- mapkit.Directions
-  eta 

Instance Method

# eta

Retrieves estimated arrival times to up to 10 destinations from a single starting point.

MapKit JS 5.46+

``` source
number eta(
 EtaRequestOptions request,
 function callback
);
```

## Parameters 

`request`  

An EtaRequestOptions object that specifies details for the server to provide estimated arrival times at one or more destinations.

`callback`  

A callback function that receives the estimated time response object, returned asynchronously.

## Return Value

A request ID, which you can pass to cancel to abort a pending request.

## Discussion

To get a set of estimated arrival times, provide an EtaRequestOptions object when you call the eta method. You may provide up to 10 destinations. The server returns an error if you request more than 10 destinations in a single request.

Estimated times are returned asynchronously via a callback function. MapKit JS invokes the callback function with two arguments, `error` on failure and `data` on success.

`error` contains an error code and a text description of the error. `data` is an EtaResponse object.

## See Also

### Getting estimated arrival times

EtaRequestOptions

The options you may provide for requesting estimated arrival times.

EtaResponse

The estimated arrival times for a set of destinations.

EtaResult

The mode of transportation, distance, and travel time estimates for a single destination.

