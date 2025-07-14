

- Metal Performance Shaders Graph
- MPSGraph
-  minimum(\_:\_:name:) 

Instance Method

# minimum(\_:\_:name:)

Returns the elementwise minimum of the input tensors.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func minimum(
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

This operation creates a minimum operation and returns the result tensor. It supports broadcasting as well.

```
resultTensor = min(primaryTensor, secondaryTensor)
```

