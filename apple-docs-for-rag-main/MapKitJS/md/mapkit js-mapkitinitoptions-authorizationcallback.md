

- MapKit JS
- MapKitInitOptions
-  authorizationCallback 

Instance Method

# authorizationCallback

A callback function that obtains a token.

MapKit JS 5.0+

``` source
void authorizationCallback(
 function done
);
```

## Parameters 

`done`  

A function that completes the MapKit JS token request. Called after creating a new token.

## Discussion

MapKit JS asyncronously invokes the `authorizationCallback` function throughout a session to obtain new authorization tokens. In the callback, you create a token and pass it to the function that MapKit JS provides in the `done` parameter.

## See Also

### Callback and language

language

An ID that indicates the preferred language to use when displaying map labels, controls, directions, and other text.

