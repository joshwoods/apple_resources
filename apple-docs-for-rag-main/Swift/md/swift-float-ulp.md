

- Swift
- Float
-  ulp 

Instance Property

# ulp

The unit in the last place of this value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var ulp: Float { get }
```

## Discussion

This is the unit of the least significant digit in this value’s significand. For most numbers `x`, this is the difference between `x` and the next greater (in magnitude) representable number. There are some edge cases to be aware of:

- If `x` is not a finite number, then `x.ulp` is NaN.

- If `x` is very small in magnitude, then `x.ulp` may be a subnormal number. If a type does not support subnormals, `x.ulp` may be rounded to zero.

- `greatestFiniteMagnitude.ulp` is a finite number, even though the next greater representable value is `infinity`.

See also the `ulpOfOne` static property.

## See Also

### Querying a Float

var significand: Float

The significand of the floating-point value.

var exponent: Int

The exponent of the floating-point value.

var nextUp: Float

The least representable value that compares greater than this value.

var nextDown: Self

The greatest representable value that compares less than this value.

var binade: Float

The floating-point value with the same sign and exponent as this value, but with a significand of 1.0.

