

- Swift
- BinaryFloatingPoint
-  binade 

Instance Property

# binade

The floating-point value with the same sign and exponent as this value, but with a significand of 1.0.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var binade: Self { get }
```

**Required**

## Discussion

A *binade* is a set of binary floating-point values that all have the same sign and exponent. The `binade` property is a member of the same binade as this value, but with a unit significand.

In this example, `x` has a value of `21.5`, which is stored as `1.34375 * 2**4`, where `**` is exponentiation. Therefore, `x.binade` is equal to `1.0 * 2**4`, or `16.0`.

```
let x = 21.5
// x.significand == 1.34375
// x.exponent == 4

let y = x.binade
// y == 16.0
// y.significand == 1.0
// y.exponent == 4
```

## See Also

### Working with Binary Representation

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

init(sign: FloatingPointSign, exponentBitPattern: Self.RawExponent, significandBitPattern: Self.RawSignificand)

Creates a new instance from the specified sign and bit patterns.

**Required**

associatedtype RawExponent : UnsignedInteger

A type that represents the encoded exponent of a value.

**Required**

associatedtype RawSignificand : UnsignedInteger

A type that represents the encoded significand of a value.

**Required**

