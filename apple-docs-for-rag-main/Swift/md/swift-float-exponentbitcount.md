

- Swift
- Float
-  exponentBitCount 

Type Property

# exponentBitCount

The number of bits used to represent the type’s exponent.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

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

## See Also

### Working with Binary Representation

var bitPattern: UInt32

The bit pattern of the value’s encoding.

var significandBitPattern: UInt32

The raw encoding of the value’s significand field.

var significandWidth: Int

The number of bits required to represent the value’s significand.

var exponentBitPattern: UInt

The raw encoding of the value’s exponent field.

static var significandBitCount: Int

The available number of fractional significand bits.

static var radix: Int

The radix, or base of exponentiation, for a floating-point type.

init(bitPattern: UInt32)

Creates a new value with the given bit pattern.

init(sign: FloatingPointSign, exponentBitPattern: UInt, significandBitPattern: UInt32)

Creates a new instance from the specified sign and bit patterns.

init(nan: Float.RawSignificand, signaling: Bool)

Creates a NaN (“not a number”) value with the specified payload.

typealias Exponent

A type that can represent any written exponent.

typealias RawSignificand

A type that represents the encoded significand of a value.

