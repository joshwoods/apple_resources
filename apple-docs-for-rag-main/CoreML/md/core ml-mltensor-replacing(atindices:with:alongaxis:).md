

- Core ML
- MLTensor
-  replacing(atIndices:with:alongAxis:) 

Instance Method

# replacing(atIndices:with:alongAxis:)

Replaces slices along the specified indices with the given replacement values.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func replacing(
    atIndices indices: MLTensor,
    with replacement: some MLTensorScalar,
    alongAxis axis: Int
) -> MLTensor
```

## Parameters 

`indices`  

A 32-bit integer tensor containing indices to scatter values from `replacement`. `indices` must have the same shape as `self` except at `axis`. Must be in the range `[-rank, rank)`.

`replacement`  

The replacement value.

`axis`  

The axis to scatter to.

## Return Value

The updated tensor.

## Discussion

For example:

```
let x = MLTensor(shape: [2, 3], scalars: [
    10, 30, 20,
    60, 40, 50
], scalarType: Float.self)
let i = MLTensor(shape: [2, 1], scalars: [
    1,
    0
], scalarType: Int32.self)
let y = x.replacing(with: 99, atIndices: i, alongAxis: 1)
// [[10, 99, 20],
//  [99, 40, 50]]
```

