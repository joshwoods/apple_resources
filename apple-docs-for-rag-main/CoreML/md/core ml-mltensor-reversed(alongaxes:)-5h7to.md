

- Core ML
- MLTensor
-  reversed(alongAxes:) 

Instance Method

# reversed(alongAxes:)

Returns a new tensor with the specified dimensions reversed.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func reversed(alongAxes axes: [Int]) -> MLTensor
```

## Parameters 

`axes`  

Axis or axes to reverse the elements of the tensor. Must be in the range `[-rank, rank)`. If no axis is specified, the tensor will be reversed along all axes.

## Return Value

A new tensor with the same shape and scalar type with the specified dimensions reversed.

## Discussion

For example:

```
let x = MLTensor(shape: [4], scalars: [0,  1,  2,  3], scalarType: Float.self)
let y = x.reversed(alongAxes: [0])
// [3, 2, 1, 0]
```

