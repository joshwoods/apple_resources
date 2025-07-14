

- Metal Performance Shaders Graph
- MPSGraph
-  conjugate(tensor:name:) 

Instance Method

# conjugate(tensor:name:)

Returns the complex conjugate of the input tensor elements.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func conjugate(
    tensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor.

`name`  

An optional string which serves as an identifier for the operation..

## Return Value

A valid `MPSGraphTensor` object containing the elementwise result of the applied operation.

