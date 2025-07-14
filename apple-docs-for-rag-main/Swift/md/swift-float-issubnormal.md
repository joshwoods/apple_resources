

- Swift
- Float
-  isSubnormal 

Instance Property

# isSubnormal

A Boolean value indicating whether the instance is subnormal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isSubnormal: Bool { get }
```

## Discussion

A *subnormal* value is a nonzero number that has a lesser magnitude than the smallest normal number. Subnormal values don’t use the full precision available to values of a type.

Zero is neither a normal nor a subnormal number. Subnormal numbers are often called *denormal* or *denormalized*—these are different names for the same concept.

## See Also

### Querying a Float’s State

var isZero: Bool

A Boolean value indicating whether the instance is equal to zero.

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

var isCanonical: Bool

A Boolean value indicating whether the instance’s representation is in its canonical form.

var floatingPointClass: FloatingPointClassification

The classification of this value.

