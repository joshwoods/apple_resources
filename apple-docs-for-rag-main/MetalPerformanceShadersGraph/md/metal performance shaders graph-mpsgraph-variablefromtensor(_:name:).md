

- Metal Performance Shaders Graph
- MPSGraph
-  variableFromTensor(\_:name:) 

Instance Method

# variableFromTensor(\_:name:)

Creates a variable from an input tensor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func variableFromTensor(
    _ tensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The tensor from which to form the variable.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

