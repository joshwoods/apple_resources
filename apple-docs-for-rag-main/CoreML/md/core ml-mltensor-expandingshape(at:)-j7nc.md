

- Core ML
- MLTensor
-  expandingShape(at:) 

Instance Method

# expandingShape(at:)

Returns a shape-expanded tensor with a dimension of 1 inserted at the specified shape indices.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func expandingShape(at axes: [Int]) -> MLTensor
```

## Parameters 

`axes`  

The axes at which to expand the shape.

## Discussion

For example:

```
let x = MLTensor(shape: [2], scalars: [1, 2], scalarType: Float.self)
let y = x.expandingShape(at: [0])
y.shape // is [1, 2]
```

