

- Metal Performance Shaders Graph
-  MPSGraphCompilationCompletionHandler 

Type Alias

# MPSGraphCompilationCompletionHandler

A notification that appears when compilation finishes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
typealias MPSGraphCompilationCompletionHandler = (MPSGraphExecutable, (any Error)?) -> Void
```

## Parameters 

`executable`  

If no error, the executable produced by the compilation.

`error`  

If an error occurs, more information might be found here.

