

- Core ML
- MLTensorRangeExpression
-  range(\_:stride:) 

Type Method

# range(\_:stride:)

Slice the tensor at the specified dimension.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func range(
    _ range: Range,
    stride: Int = 1
) -> any MLTensorRangeExpression
```

Available when `Self` is `_MLTensorRange`.

## Discussion

```
let x = MLTensor(randomNormal: [1, 3, 28, 28], scalarType: Float.self)
let y = x[..., 0..

