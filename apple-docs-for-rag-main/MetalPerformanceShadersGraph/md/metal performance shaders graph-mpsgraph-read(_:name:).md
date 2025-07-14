

- Metal Performance Shaders Graph
- MPSGraph
-  read(\_:name:) 

Instance Method

# read(\_:name:)

Creates a read op which reads at this point of execution of the graph and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func read(
    _ variable: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`variable`  

The variable resource tensor to read from.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

