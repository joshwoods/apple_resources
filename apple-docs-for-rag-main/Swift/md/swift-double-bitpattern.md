

- Swift
- Double
-  bitPattern 

Instance Property

# bitPattern

The bit pattern of the value’s encoding.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var bitPattern: UInt64 { get }
```

## Discussion

The bit pattern matches the binary interchange format defined by the IEEE 754 specification.

## See Also

### Working with Binary Representation

var significandBitPattern: UInt64

The raw encoding of the value’s significand field.

var significandWidth: Int

The number of bits required to represent the value’s significand.

var exponentBitPattern: UInt

The raw encoding of the value’s exponent field.

static var significandBitCount: Int

The available number of fractional significand bits.

static var exponentBitCount: Int

The number of bits used to represent the type’s exponent.

static var radix: Int

The radix, or base of exponentiation, for a floating-point type.

init(bitPattern: UInt64)

Creates a new value with the given bit pattern.

init(sign: FloatingPointSign, exponentBitPattern: UInt, significandBitPattern: UInt64)

Creates a new instance from the specified sign and bit patterns.

init(nan: Double.RawSignificand, signaling: Bool)

Creates a NaN (“not a number”) value with the specified payload.

typealias Exponent

A type that can represent any written exponent.

typealias RawSignificand

A type that represents the encoded significand of a value.

typealias RawExponent

A type that represents the encoded exponent of a value.

