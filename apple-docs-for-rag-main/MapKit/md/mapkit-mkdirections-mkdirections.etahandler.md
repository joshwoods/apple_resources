

- MapKit
- MKDirections
-  MKDirections.ETAHandler 

Type Alias

# MKDirections.ETAHandler

The block to use for processing travel-time information.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias ETAHandler = (MKDirections.ETAResponse?, (any Error)?) -> Void
```

## Parameters 

`response`  

The `response` parameter contains the travel-time response. If an error occurs or the framework can’t determine the travel time, this parameter is `nil`.

`error`  

The `error` parameter contains information about any errors that occur. If no errors occur, this parameter is `nil`.

## Discussion

The implementation of your block needs to check for a value in the `error` parameter and, if that parameter is `nil`, incorporate the travel-time information from the `response` parameter.

## See Also

### Getting the ETA

func calculateETA(completionHandler: MKDirections.ETAHandler)

Begins calculating the requested travel-time information asynchronously.

class ETAResponse

The travel-time information that Apple servers return.

