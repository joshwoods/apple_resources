

- Metal Performance Shaders Graph
- MPSGraph
-  modulo(\_:\_:name:) 

Instance Method

# modulo(\_:\_:name:)

Returns the remainder obtained by dividing the first input tensor by the second.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func modulo(
    _ primaryTensor: MPSGraphTensor,
    _ secondaryTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`primaryTensor`  

The LHS tensor of the binary Op.

`secondaryTensor`  

The RHS tensor of the binary Op.

`name`  

An optional string which serves as an identifier for the operation.

## Return Value

A valid `MPSGraphTensor` object containing the elementwise result of the applied operation.

## Discussion

This operation creates a modulo operation and returns the result tensor. It supports broadcasting as well.

```
resultTensor = primaryTensor % secondaryTensor
```

