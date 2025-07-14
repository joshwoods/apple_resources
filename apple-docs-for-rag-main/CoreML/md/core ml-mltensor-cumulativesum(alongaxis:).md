

- Core ML
- MLTensor
-  cumulativeSum(alongAxis:) 

Instance Method

# cumulativeSum(alongAxis:)

Computes the cumulative sum along the specified axis.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func cumulativeSum(alongAxis axis: Int = 0) -> MLTensor
```

## Parameters 

`axis`  

The axis along which to perform the cumulative sum. The default value is `0`. Must be in the range `[-rank, rank)` and have a rank greater than zero.

## Return Value

The result of the cumulative sum operation.

## Discussion

The scalar type of the tensor must be numeric.

For example:

```
MLTensor([1, 2, 3]).cumulativeSum() = [1, 1 + 2, 1 + 2 + 3]
```

