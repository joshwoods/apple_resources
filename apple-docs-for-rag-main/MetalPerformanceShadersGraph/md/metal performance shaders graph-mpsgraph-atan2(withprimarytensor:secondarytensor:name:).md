

- Metal Performance Shaders Graph
- MPSGraph
-  atan2(withPrimaryTensor:secondaryTensor:name:) 

Instance Method

# atan2(withPrimaryTensor:secondaryTensor:name:)

Returns the elementwise two-argument arctangent of the input tensors.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func atan2(
    withPrimaryTensor primaryTensor: MPSGraphTensor,
    secondaryTensor: MPSGraphTensor,
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

This operation creates a `atan2` operation and returns the result tensor. It supports broadcasting as well. Graph computes arc tangent of primaryTensor over secondaryTensor.

```
resultTensor = atan2(primaryTensor, secondaryTensor)
```

