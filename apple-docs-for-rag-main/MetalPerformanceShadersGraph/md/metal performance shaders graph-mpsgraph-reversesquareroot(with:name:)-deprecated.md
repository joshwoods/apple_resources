

- Metal Performance Shaders Graph
- MPSGraph
-  reverseSquareRoot(with:name:) Deprecated

Instance Method

# reverseSquareRoot(with:name:)

Applies the reverse square root operation to the input tensor elements.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func reverseSquareRoot(
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

The reverse square root operation is the reciprocal of the square root.

