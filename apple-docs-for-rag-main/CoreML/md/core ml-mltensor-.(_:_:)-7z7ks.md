

- Core ML
- MLTensor
-  .\|(\_:\_:) 

Operator

# .\|(\_:\_:)

Computes element-wise logical OR where both operands are expected contain Boolean scalar elements.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func .| (lhs: MLTensor, rhs: MLTensor) -> MLTensor
```

## Discussion

For example:

```
let x = MLTensor([true, true, true])
let y = MLTensor([true, false, true])
x .| y // is [true, true, true]
```

