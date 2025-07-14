

- Metal Performance Shaders Graph
- MPSGraph
-  isFinite(with:name:) 

Instance Method

# isFinite(with:name:)

Checks if the input tensor elements are finite or not.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func isFinite(
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

A valid `MPSGraphTensor` object containing the elementwise result of the applied operation.

## Discussion

If the input tensor element is finite, the operation returns `true`, else it returns `false`.

