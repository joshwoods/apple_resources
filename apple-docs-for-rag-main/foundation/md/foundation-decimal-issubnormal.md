

- Foundation
- Decimal
-  isSubnormal 

Instance Property

# isSubnormal

A Boolean value indicating whether this decimal is subnormal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isSubnormal: Bool { get }
```

## Discussion

A *subnormal* value is a nonzero number that has a lesser magnitude than the smallest normal number. Subnormal values do not use the full precision available to values of a type.

Zero is neither a normal nor a subnormal number. Subnormal numbers are often called *denormal* or *denormalized*—these are different names for the same concept.

## See Also

### Getting a decimal’s characteristics

var sign: FloatingPointSign

The sign of the decimal.

var exponent: Int

The exponent of the decimal.

var significand: Decimal

The significand of the decimal.

var floatingPointClass: FloatingPointClassification

The IEEE 754 class of this type.

var isCanonical: Bool

A Boolean value indicating whether the representation of this decimal is canonical.

var isFinite: Bool

A Boolean value indicating whether this decimal is zero, subnormal, or normal (not infinity or NaN).

var isInfinite: Bool

A Boolean value indicating whether this decimal is infinity.

var isNaN: Bool

A Boolean value indicating whether this decimal is NaN.

var isNormal: Bool

A Boolean value indicating whether this decimal is normal (not zero, subnormal, infinity, or NaN).

var isSignMinus: Bool

A Boolean value indicating whether this decimal has a negative sign.

var isSignaling: Bool

A Boolean value indicating whether this decimal is a signaling NaN.\`\`

var isSignalingNaN: Bool

A Boolean value indicating whether this decimal is a signaling NaN.

var isZero: Bool

A Boolean value indicating whether this value is zero.

var nextDown: Decimal

The greatest representable value that is less than this decimal.

var nextUp: Decimal

The least representable value that is greater than this decimal.

