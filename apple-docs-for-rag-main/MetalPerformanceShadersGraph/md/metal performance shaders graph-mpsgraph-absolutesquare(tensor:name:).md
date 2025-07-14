

- Metal Performance Shaders Graph
- MPSGraph
-  absoluteSquare(tensor:name:) 

Instance Method

# absoluteSquare(tensor:name:)

Returns the absolute square of the input tensor elements.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func absoluteSquare(
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

