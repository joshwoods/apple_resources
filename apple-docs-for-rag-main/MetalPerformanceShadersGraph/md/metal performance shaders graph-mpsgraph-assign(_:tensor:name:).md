

- Metal Performance Shaders Graph
- MPSGraph
-  assign(\_:tensor:name:) 

Instance Method

# assign(\_:tensor:name:)

Creates an assign operation which writes at this point of execution of the graph.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func assign(
    _ variable: MPSGraphTensor,
    tensor: MPSGraphTensor,
    name: String?
) -> MPSGraphOperation
```

## Parameters 

`variable`  

The variable resource tensor to assign to.

`tensor`  

The tensor to assign to the variable.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

