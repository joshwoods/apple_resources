

- Swift
- BinaryFloatingPoint
-  exponentBitCount 

Type Property

# exponentBitCount

The number of bits used to represent the type’s exponent.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var exponentBitCount: Int { get }
```

**Required**

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

## See Also

### Working with Binary Representation

var binade: Self

The floating-point value with the same sign and exponent as this value, but with a significand of 1.0.

**Required**

var exponentBitPattern: Self.RawExponent

The raw encoding of the value’s exponent field.

**Required**

var significandBitPattern: Self.RawSignificand

The raw encoding of the value’s significand field.

**Required**

var significandWidth: Int

The number of bits required to represent the value’s significand.

**Required**

static var significandBitCount: Int

The available number of fractional significand bits.

**Required**

init(sign: FloatingPointSign, exponentBitPattern: Self.RawExponent, significandBitPattern: Self.RawSignificand)

Creates a new instance from the specified sign and bit patterns.

**Required**

associatedtype RawExponent : UnsignedInteger

A type that represents the encoded exponent of a value.

**Required**

associatedtype RawSignificand : UnsignedInteger

A type that represents the encoded significand of a value.

**Required**

