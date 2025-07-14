

- Core ML
- MLTensor
-  .!=(\_:\_:) 

Operator

# .!=(\_:\_:)

Computes element-wise inequality between two tensors.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func .!= (lhs: MLTensor, rhs: MLTensor) -> MLTensor
```

## Return Value

A Boolean tensor where each element is true if `self` is not equal to than the corresponding element of `other`, and false otherwise.

## Discussion

Shapes must be broadcastable, where the broadcasted shape becomes the shape of the output.

