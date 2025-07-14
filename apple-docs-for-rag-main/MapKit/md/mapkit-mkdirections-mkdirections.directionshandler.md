

- MapKit
- MKDirections
-  MKDirections.DirectionsHandler 

Type Alias

# MKDirections.DirectionsHandler

The block to use for processing the requested route information.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias DirectionsHandler = (MKDirections.Response?, (any Error)?) -> Void
```

## Parameters 

`response`  

The `response` parameter contains the route information for the request. If an error occurs or the framework can’t determine a route, this parameter is `nil`.

`error`  

The `error` parameter contains information about any errors that occur. If no errors occur, this parameter is `nil`.

## Discussion

The implementation of your block needs to check for a value in the `error` parameter and, if that parameter is `nil`, incorporate the route information from the `response` parameter.

## See Also

### Getting the directions

func calculate(completionHandler: MKDirections.DirectionsHandler)

Begins calculating the requested route information asynchronously.

class Response

The route information that Apple servers return in response to your request for directions.

