

- Swift
- Float80
-  significand 

Instance Property

# significand

The significand of the floating-point value.

macOS 10.10+

``` source
var significand: Float80 { get }
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

