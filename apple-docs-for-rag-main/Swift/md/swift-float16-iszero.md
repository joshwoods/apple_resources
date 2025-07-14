

- Swift
- Float16
-  isZero 

Instance Property

# isZero

A Boolean value indicating whether the instance is equal to zero.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var isZero: Bool { get }
```

## Discussion

The `isZero` property of a value `x` is `true` when `x` represents either `-0.0` or `+0.0`. `x.isZero` is equivalent to the following comparison: `x == 0.0`.

```
let x = -0.0
x.isZero        // true
x == 0.0        // true
```

