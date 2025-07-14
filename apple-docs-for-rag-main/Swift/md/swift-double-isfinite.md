

- Swift
- Double
-  isFinite 

Instance Property

# isFinite

A Boolean value indicating whether this instance is finite.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isFinite: Bool { get }
```

## Discussion

All values other than NaN and infinity are considered finite, whether normal or subnormal. For NaN, both `isFinite` and `isInfinite` are false.

## See Also

### Querying a Double’s State

var isZero: Bool

A Boolean value indicating whether the instance is equal to zero.

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

