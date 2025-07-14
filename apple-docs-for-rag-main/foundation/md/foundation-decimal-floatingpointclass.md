

- Foundation
- Decimal
-  floatingPointClass 

Instance Property

# floatingPointClass

The IEEE 754 class of this type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var floatingPointClass: FloatingPointClassification { get }
```

## See Also

### Getting a decimal’s characteristics

var sign: FloatingPointSign

The sign of the decimal.

var exponent: Int

The exponent of the decimal.

var significand: Decimal

The significand of the decimal.

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

var isSubnormal: Bool

A Boolean value indicating whether this decimal is subnormal.

var isZero: Bool

A Boolean value indicating whether this value is zero.

var nextDown: Decimal

The greatest representable value that is less than this decimal.

var nextUp: Decimal

The least representable value that is greater than this decimal.

