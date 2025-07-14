

- Swift
- Float
-  nextUp 

Instance Property

# nextUp

The least representable value that compares greater than this value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var nextUp: Float { get }
```

## Discussion

For any finite value `x`, `x.nextUp` is greater than `x`. For `nan` or `infinity`, `x.nextUp` is `x` itself. The following special cases also apply:

- If `x` is `-infinity`, then `x.nextUp` is `-greatestFiniteMagnitude`.

- If `x` is `-leastNonzeroMagnitude`, then `x.nextUp` is `-0.0`.

- If `x` is zero, then `x.nextUp` is `leastNonzeroMagnitude`.

- If `x` is `greatestFiniteMagnitude`, then `x.nextUp` is `infinity`.

## See Also

### Querying a Float

var ulp: Float

The unit in the last place of this value.

var significand: Float

The significand of the floating-point value.

var exponent: Int

The exponent of the floating-point value.

var nextDown: Self

The greatest representable value that compares less than this value.

var binade: Float

The floating-point value with the same sign and exponent as this value, but with a significand of 1.0.

