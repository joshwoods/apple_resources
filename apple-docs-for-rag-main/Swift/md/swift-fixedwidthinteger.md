

- Swift
-  FixedWidthInteger 

Protocol

# FixedWidthInteger

An integer type that uses a fixed size for every instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol FixedWidthInteger : BinaryInteger, LosslessStringConvertible where Self.Magnitude : FixedWidthInteger, Self.Magnitude : UnsignedInteger, Self.Stride : FixedWidthInteger, Self.Stride : SignedInteger
```

## Overview

The `FixedWidthInteger` protocol adds binary bitwise operations, bit shifts, and overflow handling to the operations supported by the `BinaryInteger` protocol.

Use the `FixedWidthInteger` protocol as a constraint or extension point when writing operations that depend on bit shifting, performing bitwise operations, catching overflows, or having access to the maximum or minimum representable value of a type. For example, the following code provides a `binaryString` property on every fixed-width integer that represents the number’s binary representation, split into 8-bit chunks.

```
extension FixedWidthInteger {
    var binaryString: String {
        var result: [String] = []
        for i in 0..> (i * 8))
            let byteString = String(byte, radix: 2)
            let padding = String(repeating: "0",
                                 count: 8 - byteString.count)
            result.append(padding + byteString)
        }
        return "0b" + result.reversed().joined(separator: "_")
    }
}

print(Int16.max.binaryString)
// Prints "0b01111111_11111111"
print((101 as UInt8).binaryString)
// Prints "0b01100101"
```

The `binaryString` implementation uses the static `bitWidth` property and the right shift operator (`>>`), both of which are available to any type that conforms to the `FixedWidthInteger` protocol.

The next example declares a generic `squared` function, which accepts an instance `x` of any fixed-width integer type. The function uses the `multipliedReportingOverflow(by:)` method to multiply `x` by itself and check whether the result is too large to represent in the same type.

```
func squared(_ x: T) -> T? {
    let (result, overflow) = x.multipliedReportingOverflow(by: x)
    if overflow {
        return nil
    }
    return result
}

let (x, y): (Int8, Int8) = (9, 123)
print(squared(x))
// Prints "Optional(81)"
print(squared(y))
// Prints "nil"
```

# Conforming to the FixedWidthInteger Protocol

To make your own custom type conform to the `FixedWidthInteger` protocol, declare the required initializers, properties, and methods. The required methods that are suffixed with `ReportingOverflow` serve as the customization points for arithmetic operations. When you provide just those methods, the standard library provides default implementations for all other arithmetic methods and operators.

## Topics

### Operators

static func &amp;* (Self, Self) -> Self

Returns the product of the two given values, wrapping the result in case of any overflow.

**Required** Default implementation provided.

static func &amp;*= (inout Self, Self)

Multiplies two values and stores the result in the left-hand-side variable, wrapping any overflow.

static func &amp;+ (Self, Self) -> Self

Returns the sum of the two given values, wrapping the result in case of any overflow.

static func &amp;+= (inout Self, Self)

Adds two values and stores the result in the left-hand-side variable, wrapping any overflow.

static func &amp;- (Self, Self) -> Self

Returns the difference of the two given values, wrapping the result in case of any overflow.

static func &amp;-= (inout Self, Self)

Subtracts the second value from the first and stores the difference in the left-hand-side variable, wrapping any overflow.

static func &amp;>> (Self, Self) -> Self

Returns the result of shifting a value’s binary representation the specified number of digits to the right, masking the shift amount to the type’s bit width.

**Required** Default implementations provided.

static func &amp;&lt;&lt; (Self, Self) -> Self

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width.

**Required** Default implementations provided.

static func &amp;>>= (inout Self, Self)

Calculates the result of shifting a value’s binary representation the specified number of digits to the right, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

**Required** Default implementation provided.

static func &amp;&lt;&lt;= (inout Self, Self)

Returns the result of shifting a value’s binary representation the specified number of digits to the left, masking the shift amount to the type’s bit width, and stores the result in the left-hand-side variable.

**Required** Default implementation provided.

### Initializers

init?&lt;S>(S, radix: Int)

Creates a new integer value from the given string and radix.

init(bigEndian: Self)

Creates an integer from its big-endian representation, changing the byte order if necessary.

**Required** Default implementation provided.

init(littleEndian: Self)

Creates an integer from its little-endian representation, changing the byte order if necessary.

**Required** Default implementation provided.

### Instance Properties

var bigEndian: Self

The big-endian representation of this integer.

**Required** Default implementation provided.

var byteSwapped: Self

A representation of this integer with the byte order swapped.

**Required**

var leadingZeroBitCount: Int

The number of leading zeros in this value’s binary representation.

**Required**

var littleEndian: Self

The little-endian representation of this integer.

**Required** Default implementation provided.

var nonzeroBitCount: Int

The number of bits equal to 1 in this value’s binary representation.

**Required**

### Instance Methods

func addingReportingOverflow(Self) -> (partialValue: Self, overflow: Bool)

Returns the sum of this value and the given value, along with a Boolean value indicating whether overflow occurred in the operation.

**Required**

func dividedReportingOverflow(by: Self) -> (partialValue: Self, overflow: Bool)

Returns the quotient obtained by dividing this value by the given value, along with a Boolean value indicating whether overflow occurred in the operation.

**Required**

func dividingFullWidth((high: Self, low: Self.Magnitude)) -> (quotient: Self, remainder: Self)

Returns a tuple containing the quotient and remainder obtained by dividing the given value by this value.

**Required**

func multipliedFullWidth(by: Self) -> (high: Self, low: Self.Magnitude)

Returns a tuple containing the high and low parts of the result of multiplying this value by the given value.

**Required** Default implementation provided.

func multipliedReportingOverflow(by: Self) -> (partialValue: Self, overflow: Bool)

Returns the product of this value and the given value, along with a Boolean value indicating whether overflow occurred in the operation.

**Required**

func remainderReportingOverflow(dividingBy: Self) -> (partialValue: Self, overflow: Bool)

Returns the remainder after dividing this value by the given value, along with a Boolean value indicating whether overflow occurred during division.

**Required**

func subtractingReportingOverflow(Self) -> (partialValue: Self, overflow: Bool)

Returns the difference obtained by subtracting the given value from this value, along with a Boolean value indicating whether overflow occurred in the operation.

**Required**

### Type Properties

static var bitWidth: Int

The number of bits used for the underlying binary representation of values of this type.

**Required** Default implementation provided.

static var max: Self

The maximum representable integer in this type.

**Required**

static var min: Self

The minimum representable integer in this type.

**Required**

### Type Methods

static func random(in: Range&lt;Self>) -> Self

Returns a random value within the specified range.

static func random(in: ClosedRange&lt;Self>) -> Self

Returns a random value within the specified range.

static func random&lt;T>(in: Range&lt;Self>, using: inout T) -> Self

Returns a random value within the specified range, using the given generator as a source for randomness.

static func random&lt;T>(in: ClosedRange&lt;Self>, using: inout T) -> Self

Returns a random value within the specified range, using the given generator as a source for randomness.

## Relationships

### Inherits From

- AdditiveArithmetic
- BinaryInteger
- Comparable
- CustomStringConvertible
- Equatable
- ExpressibleByIntegerLiteral
- Hashable
- LosslessStringConvertible
- Numeric
- Strideable

### Conforming Types

- Int
- Int128
- Int16
- Int32
- Int64
- Int8
- UInt
- UInt128
- UInt16
- UInt32
- UInt64
- UInt8

## See Also

### Integer

protocol BinaryInteger

An integer type with a binary representation.

protocol SignedInteger

An integer type that can represent both positive and negative values.

protocol UnsignedInteger

An integer type that can represent only nonnegative values.

