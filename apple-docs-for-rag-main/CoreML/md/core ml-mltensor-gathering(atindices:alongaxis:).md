

- Core ML
- MLTensor
-  gathering(atIndices:alongAxis:) 

Instance Method

# gathering(atIndices:alongAxis:)

Returns a tensor by gathering slices along the given axis at the specified indices.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func gathering(
    atIndices indices: MLTensor,
    alongAxis axis: Int
) -> MLTensor
```

## Parameters 

`indices`  

A 32-bit integer tensor containing indices to gather at.

`axis`  

The dimension to gather along. Must be in the range `[-rank, rank)`.

## Return Value

The gathered tensor.

## Discussion

For example:

```
let x = MLTensor(shape: [3, 3], scalars: [
     0,  1,  2,
    10, 11, 12,
    20, 21, 22
], scalarType: Float.self)
let i = MLTensor([2, 1], scalarType: Int32.self)
let y0 = x.gathering(atIndices: i)
// [[20, 21, 22],
//  [10, 11, 12]]

let y1 = x.gathering(atIndices: i, alongAxis: 1)
// [[ 2,  1],
//  [12, 11],
//  [22, 21]]
```

