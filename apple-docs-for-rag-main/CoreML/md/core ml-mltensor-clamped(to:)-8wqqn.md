

- Core ML
- MLTensor
-  clamped(to:) 

Instance Method

# clamped(to:)

Clamps all elements to the given lower and upper bounds, inclusively.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func clamped(to bounds: ClosedRange) -> MLTensor
```

## Discussion

For example:

```
let x = MLTensor([-1.0, 1.0, 2.0])
let y = x.clamped(to: 0...1)
await y.shapedArray(of: Float.self) // is [0.0, 1.0, 1.0]
```

