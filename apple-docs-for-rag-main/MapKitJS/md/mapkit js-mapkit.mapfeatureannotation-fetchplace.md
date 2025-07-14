

- MapKit JS
- mapkit.MapFeatureAnnotation
-  fetchPlace 

Instance Method

# fetchPlace

Fetches the place object associated with the map feature.

MapKit JS 5.74+

``` source
number fetchPlace(
 function|FetchDelegate callback
);
```

## Parameters 

`callback`  

Required. The framework invokes appropriate methods on FetchDelegate, or the callback function with two arguments, `error` and `data,` on success or failure:

- error — Contains an error code and a message that describes the error.

- data — A data object that contains an array with one Place object associated with the map feature, or an empty array if the server can’t return the specified place.

