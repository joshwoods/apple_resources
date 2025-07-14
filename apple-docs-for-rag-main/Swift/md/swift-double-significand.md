

- Swift
- Double
-  significand 

Instance Property

# significand

The significand of the floating-point value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var significand: Double { get }
```

## Discussion

The magnitude of a floating-point value `x` of type `F` can be calculated by using the following formula, where `**` is exponentiation:

```
x.significand * (F.radix ** x.exponent)
```

In the next example, `y` has a value of `21.5`, which is encoded as `1.34375 * 2 ** 4`. The significand of `y` is therefore 1.34375.

```
let y: Double = 21.5
// y.significand == 1.34375
// y.exponent == 4
// Double.radix == 2
```

If a type’s radix is 2, then for finite nonzero numbers, the significand is in the range `1.0 ..IEEE 754 specification, to allay confusion with the use of mantissa for the fractional part of a logarithm.

## See Also

### Querying a Double

var ulp: Double

The unit in the last place of this value.

var exponent: Int

The exponent of the floating-point value.

var nextUp: Double

The least representable value that compares greater than this value.

var nextDown: Self

The greatest representable value that compares less than this value.

var binade: Double

The floating-point value with the same sign and exponent as this value, but with a significand of 1.0.

