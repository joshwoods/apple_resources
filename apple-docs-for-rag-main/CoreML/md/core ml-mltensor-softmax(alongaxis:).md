

- Core ML
- MLTensor
-  softmax(alongAxis:) 

Instance Method

# softmax(alongAxis:)

Computes the softmax of the specified tensor along the specified axis.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func softmax(alongAxis axis: Int = -1) -> MLTensor
```

## Parameters 

`axis`  

The axis along which softmax will be computed.

## Return Value

A new tensor with the same shape and scalar type.

