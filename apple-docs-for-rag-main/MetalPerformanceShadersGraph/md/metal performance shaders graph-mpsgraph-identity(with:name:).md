

- Metal Performance Shaders Graph
- MPSGraph
-  identity(with:name:) 

Instance Method

# identity(with:name:)

Copies the input tensor values into the output, behaving as an identity operation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func identity(
    with tensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor.

`name`  

An optional string which serves as an identifier for the operation.

## Return Value

A valid `MPSGraphTensor` object which is a copy of the input.

