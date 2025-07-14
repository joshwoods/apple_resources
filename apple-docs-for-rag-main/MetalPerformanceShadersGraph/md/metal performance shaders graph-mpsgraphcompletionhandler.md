

- Metal Performance Shaders Graph
-  MPSGraphCompletionHandler 

Type Alias

# MPSGraphCompletionHandler

A notification that appears when graph execution finishes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
typealias MPSGraphCompletionHandler = ([MPSGraphTensor : MPSGraphTensorData], (any Error)?) -> Void
```

## Parameters 

`resultsDictionary`  

If no error, the results dictionary produced by the graph operation.

`error`  

If an error occurs, more information might be found here.

