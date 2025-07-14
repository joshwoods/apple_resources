

- Core ML
- MLTensorRangeExpression
-  index(\_:) 

Type Method

# index(\_:)

Slice the tensor at the specified dimension.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func index(_ index: Int) -> any MLTensorRangeExpression
```

Available when `Self` is `_MLTensorRange`.

## Discussion

For example:

```
let x = MLTensor(randomNormal: [1, 3, 28, 28], scalarType: Float.self)
let y = x[..., 0] // or x[..., .index(0)]
y.shape // is [1, 3, 28]
```

