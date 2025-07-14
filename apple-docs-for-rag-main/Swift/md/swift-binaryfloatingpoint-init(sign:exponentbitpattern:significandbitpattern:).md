

- Swift
- BinaryFloatingPoint
-  init(sign:exponentBitPattern:significandBitPattern:) 

Initializer

# init(sign:exponentBitPattern:significandBitPattern:)

Creates a new instance from the specified sign and bit patterns.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    sign: FloatingPointSign,
    exponentBitPattern: Self.RawExponent,
    significandBitPattern: Self.RawSignificand
)
```

**Required**

## Parameters 

`sign`  

The sign of the new value.

`exponentBitPattern`  

The bit pattern to use for the exponent field of the new value.

`significandBitPattern`  

The bit pattern to use for the significand field of the new value.

## Discussion

The values passed as `exponentBitPattern` and `significandBitPattern` are interpreted in the binary interchange format defined by the IEEE 754 specification.

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

static var exponentBitCount: Int

The number of bits used to represent the type’s exponent.

**Required**

static var significandBitCount: Int

The available number of fractional significand bits.

**Required**

associatedtype RawExponent : UnsignedInteger

A type that represents the encoded exponent of a value.

**Required**

associatedtype RawSignificand : UnsignedInteger

A type that represents the encoded significand of a value.

**Required**

