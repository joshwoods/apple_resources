

- Metal Performance Shaders Graph
-  MPSGraphScheduledHandler 

Type Alias

# MPSGraphScheduledHandler

A notification that appears when graph execution schedules.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
typealias MPSGraphScheduledHandler = ([MPSGraphTensor : MPSGraphTensorData], (any Error)?) -> Void
```

## Parameters 

`resultsDictionary`  

If no error, the results dictionary produced by the graph operation. If Graph has not yet allocated, the results will be `NSNull`.

`error`  

If an error occurs, more information might be found here.

