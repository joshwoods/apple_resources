

- Metal Performance Shaders Graph
- MPSGraph
-  clamp(\_:min:max:name:) 

Instance Method

# clamp(\_:min:max:name:)

Clamps the values in the first tensor between the corresponding values in the minimum and maximum value tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func clamp(
    _ tensor: MPSGraphTensor,
    min minValueTensor: MPSGraphTensor,
    max maxValueTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The tensor to be clamped.

`minValueTensor`  

The tensor with min values to clamp to.

`name`  

An optional string which serves as an identifier for the operation.

## Return Value

A valid `MPSGraphTensor` object containing the elementwise result of the applied operation.

## Discussion

This operation creates a clamp operation and returns the result tensor. It supports broadcasting as well.

```
resultTensor = clamp(tensor, minValueTensor, maxValueTensor)
```

