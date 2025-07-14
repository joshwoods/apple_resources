

- Swift
- Double
-  nextDown 

Instance Property

# nextDown

The greatest representable value that compares less than this value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var nextDown: Self { get }
```

## Discussion

For any finite value `x`, `x.nextDown` is less than `x`. For `nan` or `-infinity`, `x.nextDown` is `x` itself. The following special cases also apply:

- If `x` is `infinity`, then `x.nextDown` is `greatestFiniteMagnitude`.

- If `x` is `leastNonzeroMagnitude`, then `x.nextDown` is `0.0`.

- If `x` is zero, then `x.nextDown` is `-leastNonzeroMagnitude`.

- If `x` is `-greatestFiniteMagnitude`, then `x.nextDown` is `-infinity`.

## See Also

### Querying a Double

var ulp: Double

The unit in the last place of this value.

var significand: Double

The significand of the floating-point value.

var exponent: Int

The exponent of the floating-point value.

var nextUp: Double

The least representable value that compares greater than this value.

var binade: Double

The floating-point value with the same sign and exponent as this value, but with a significand of 1.0.

