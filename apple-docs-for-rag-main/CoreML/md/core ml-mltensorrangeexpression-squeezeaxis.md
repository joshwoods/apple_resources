

- Core ML
- MLTensorRangeExpression
-  squeezeAxis 

Type Property

# squeezeAxis

Squeeze the tensor at the specified dimension.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static var squeezeAxis: any MLTensorRangeExpression { get }
```

Available when `Self` is `_MLTensorRange`.

## Discussion

For example:

```
let x = MLTensor(randomNormal: [1, 3, 28, 28], scalarType: Float.self)
let y = x[.squeezeAxis, ...]
y.shape // is [3, 28, 28]
```

