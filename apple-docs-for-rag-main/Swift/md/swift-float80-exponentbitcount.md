

- Swift
- Float80
-  exponentBitCount 

Type Property

# exponentBitCount

The number of bits used to represent the type’s exponent.

macOS 10.10+

``` source
static var exponentBitCount: Int { get }
```

## Discussion

A binary floating-point type’s `exponentBitCount` imposes a limit on the range of the exponent for normal, finite values. The *exponent bias* of a type `F` can be calculated as the following, where `**` is exponentiation:

```
let bias = 2 ** (F.exponentBitCount - 1) - 1
```

The least normal exponent for values of the type `F` is `1 - bias`, and the largest finite exponent is `bias`. An all-zeros exponent is reserved for subnormals and zeros, and an all-ones exponent is reserved for infinity and NaN.

For example, the `Float` type has an `exponentBitCount` of 8, which gives an exponent bias of `127` by the calculation above.

```
let bias = 2 ** (Float.exponentBitCount - 1) - 1
// bias == 127
print(Float.greatestFiniteMagnitude.exponent)
// Prints "127"
print(Float.leastNormalMagnitude.exponent)
// Prints "-126"
```

