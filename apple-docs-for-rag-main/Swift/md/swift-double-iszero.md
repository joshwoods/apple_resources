

- Swift
- Double
-  isZero 

Instance Property

# isZero

A Boolean value indicating whether the instance is equal to zero.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

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

## See Also

### Querying a Double’s State

var isFinite: Bool

A Boolean value indicating whether this instance is finite.

var isInfinite: Bool

A Boolean value indicating whether the instance is infinite.

var isNaN: Bool

A Boolean value indicating whether the instance is NaN (“not a number”).

var isSignalingNaN: Bool

A Boolean value indicating whether the instance is a signaling NaN.

var isNormal: Bool

A Boolean value indicating whether this instance is normal.

var isSubnormal: Bool

A Boolean value indicating whether the instance is subnormal.

var isCanonical: Bool

A Boolean value indicating whether the instance’s representation is in its canonical form.

var floatingPointClass: FloatingPointClassification

The classification of this value.

