

- Swift
- BinaryFloatingPoint
-  significandBitCount 

Type Property

# significandBitCount

The available number of fractional significand bits.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var significandBitCount: Int { get }
```

**Required**

## Discussion

For fixed-width floating-point types, this is the actual number of fractional significand bits.

For extensible floating-point types, `significandBitCount` should be the maximum allowed significand width (without counting any leading integral bit of the significand). If there is no upper limit, then `significandBitCount` should be `Int.max`.

Note that `Float80.significandBitCount` is 63, even though 64 bits are used to store the significand in the memory representation of a `Float80` (unlike other floating-point types, `Float80` explicitly stores the leading integral significand bit, but the `BinaryFloatingPoint` APIs provide an abstraction so that users don’t need to be aware of this detail).

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

init(sign: FloatingPointSign, exponentBitPattern: Self.RawExponent, significandBitPattern: Self.RawSignificand)

Creates a new instance from the specified sign and bit patterns.

**Required**

associatedtype RawExponent : UnsignedInteger

A type that represents the encoded exponent of a value.

**Required**

associatedtype RawSignificand : UnsignedInteger

A type that represents the encoded significand of a value.

**Required**

