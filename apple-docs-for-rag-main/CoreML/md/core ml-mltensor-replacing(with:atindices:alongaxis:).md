

- Core ML
- MLTensor
-  replacing(with:atIndices:alongAxis:) 

Instance Method

# replacing(with:atIndices:alongAxis:)

Replaces slices along the specified indices with the given replacement values.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func replacing(
    with replacement: MLTensor,
    atIndices indices: MLTensor,
    alongAxis axis: Int
) -> MLTensor
```

## Parameters 

`replacement`  

The replacement values.

`indices`  

A 32-bit integer tensor containing indices to scatter values from `replacement`. Must have the same shape as `replacement`. Must have the same shape as `self` except at `axis`.

`axis`  

The axis to scatter to. Must be in the range `[-rank, rank)`.

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
let updates = MLTensor(shape: [2, 1], scalars: [
    99,
    99
], scalarType: Float.self)
let y = x.replacing(atIndices: i, with: updates, alongAxis: 1)
// [[10, 99, 20],
//  [99, 40, 50]]
```

