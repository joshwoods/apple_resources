

- Metal Performance Shaders Graph
- MPSGraph
-  signbit(with:name:) 

Instance Method

# signbit(with:name:)

Returns the sign bit of the input tensor elements.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func signbit(
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

This operation returns `true` if the sign bit is set for the correspnding floating-point input element, otherwise it returns `false`.

