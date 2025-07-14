

- Vision
-  VNRequestProgressHandler 

Type Alias

# VNRequestProgressHandler

A block executed at intervals during the processing of a Vision request.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
typealias VNRequestProgressHandler = (VNRequest, Double, (any Error)?) -> Void
```

## Parameters 

`request`  

The completed Vision request. The results of the request, if no error occurred, reside in the results array of the request.

`fractionCompleted`  

The fraction of the request that is completed, reported between `0.0` and `1.0`. If the indeterminate property is set, this value is undefined.

`error`  

The error that caused the request to fail, or nil if the request completed successfully.

## Discussion

Vision may populate the results array in the request with partial data, before all results are ready.

Note

The Vision framework may call the progress handler on a different dispatch queue from the thread on which you initiated the original request, so ensure that your handler can execute asynchronously, in a thread-safe manner.

## See Also

### Request progress tracking

protocol VNRequestProgressProviding

A protocol for providing progress information on long-running tasks in Vision.

