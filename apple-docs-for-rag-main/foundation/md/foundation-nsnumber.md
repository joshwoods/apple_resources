

- Foundation
-  NSNumber 

Class

# NSNumber

An object wrapper for primitive scalar numeric values.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSNumber
```

## Mentioned in 

Implementing Handoff in Your App

## Overview

`NSNumber` is a subclass of `NSValue` that offers a value as any C scalar (numeric) type. It defines a set of methods specifically for setting and accessing the value as a signed or unsigned `char`, `short int`, `int`, `long int`, `long long int`, `float`, or `double` or as a `BOOL`. (Note that number objects do not necessarily preserve the type they are created with.) It also defines a compare(_:) method to determine the ordering of two `NSNumber` objects.

`NSNumber` is “toll-free bridged” with its Core Foundation counterparts: CFNumber for integer and floating point values, and CFBoolean for Boolean values. See Toll-Free Bridging for more information on toll-free bridging.

### Value Conversions

`NSNumber` provides readonly properties that return the object’s stored value converted to a particular Boolean, integer, unsigned integer, or floating point C scalar type. Because numeric types have different storage capabilities, attempting to initialize with a value of one type and access the value of another type may produce an erroneous result—for example, initializing with a `double` value exceeding `FLT_MAX` and accessing its floatValue, or initializing with an negative integer value and accessing its uintValue. In some cases, attempting to initialize with a value of a type and access the value of another type may result in loss of precision—for example, initializing with a `double` value with many significant digits and accessing its floatValue, or initializing with a large integer value and accessing its int8Value.

An `NSNumber` object initialized with a value of a particular type accessing the converted value of a different *kind* of type, such as `unsigned int` and `float`, will convert its stored value to that converted type in the following ways:

| `Value` | boolValue | intValue | uintValue | floatValue |
|----|----|----|----|----|
| false | false | `0` | `0` | `0.0` |
| true | true | `1` | `1` | `1.0` |

| `Value` | boolValue | intValue | uintValue | floatValue |
|----|----|----|----|----|
| `0` | false | `0` | `0` | `0.0` |
| `1` | true | `1` | `1` | `1.0` |
| `-1` | true | `-1` | *invalid, erroneous result* | `-1.0` |

| `Value` | boolValue | intValue | uintValue | floatValue |
|----|----|----|----|----|
| `0` | false | `0` | `0` | `0.0` |
| `1` | true | `1` | `1` | `1.0` |

| `Value` | boolValue | intValue | uintValue | floatValue |
|----|----|----|----|----|
| `0.0` | false | `0` | `0` | `0.0` |
| `1.0` | true | `1` | `1` | `1.0` |
| `-1.0` | true | `-1` | *invalid, erroneous result* | `-1.0` |

### Subclassing Notes

As with any class cluster, subclasses of `NSNumber` must override the primitive methods of its superclass, `NSValue`. In addition, there are two requirements around the data type your subclass represents:

1.  Your implementation of objCType must return one of “`c`”, “`C`”, “`s`”, “`S`”, “`i`”, “`I`”, “`l`”, “`L`”, “`q`”, “`Q`”, “`f`”, and “`d`”. This is required for the other methods of NSNumber to behave correctly.

2.  Your subclass must override the accessor method that corresponds to the declared type—for example, if your implementation of objCType returns “`i`”, you must override int32Value.

## Topics

### Initializing an NSNumber Object

init(value: Bool)

Returns an `NSNumber` object initialized to contain a given value, treated as a `BOOL`.

init(value: CChar)

Returns an `NSNumber` object initialized to contain a given value, treated as a signed `char`.

init(value: Double)

Returns an `NSNumber` object initialized to contain `value`, treated as a `double`.

init(value: Float)

Returns an `NSNumber` object initialized to contain a given value, treated as a `float`.

init(value: Int32)

Returns an `NSNumber` object initialized to contain a given value, treated as a signed `int`.

init(value: Int)

Returns an `NSNumber` object initialized to contain a given value, treated as an `NSInteger`.

init(value: Int64)

Returns an `NSNumber` object initialized to contain `value`, treated as a signed `long long`.

init(value: Int16)

Returns an `NSNumber` object initialized to contain a given value, treated as a signed `short`.

init(value: UInt8)

Returns an `NSNumber` object initialized to contain a given value, treated as an `unsigned char`.

init(value: UInt32)

Returns an `NSNumber` object initialized to contain a given value, treated as an `unsigned int`.

init(value: UInt)

Returns an `NSNumber` object initialized to contain a given value, treated as an `NSUInteger`.

init(value: UInt64)

Returns an `NSNumber` object initialized to contain a given value, treated as an `unsigned long long`.

init(value: UInt16)

Returns an `NSNumber` object initialized to contain a given value, treated as an `unsigned short`.

### Accessing Numeric Values

var boolValue: Bool

The number object’s value expressed as a Boolean value.

var int8Value: CChar

The number object’s value expressed as a `char`.

var decimalValue: Decimal

The number object’s value expressed as an Decimal structure.

var doubleValue: Double

The number object’s value expressed as a `double`, converted as necessary.

var floatValue: Float

The number object’s value expressed as a `float`, converted as necessary.

var int32Value: Int32

The number object’s value expressed as an `int`, converted as necessary.

var intValue: Int

The number object’s value expressed as an `NSInteger` object, converted as necessary.

var int64Value: Int64

The number object’s value expressed as a `long long`, converted as necessary.

var int16Value: Int16

The number object’s value expressed as a `short`, converted as necessary.

var uint8Value: UInt8

The number object’s value expressed as an unsigned `char`, converted as necessary.

var uintValue: UInt

The number object’s value expressed as an `NSUInteger` object, converted as necessary.

var uint32Value: UInt32

The number object’s value expressed as an unsigned `int`, converted as necessary.

var uint64Value: UInt64

The number object’s value expressed as an unsigned `long long`, converted as necessary.

var uint16Value: UInt16

The number object’s value expressed as an unsigned `short`, converted as necessary.

### Retrieving String Representations

func description(withLocale: Any?) -> String

var stringValue: String

The number object’s value expressed as a human-readable string.

### Comparing NSNumber Objects

func compare(NSNumber) -> ComparisonResult

Returns an `NSComparisonResult` value that indicates whether the number object’s value is greater than, equal to, or less than a given number.

func isEqual(to: NSNumber) -> Bool

Returns a Boolean value that indicates whether the number object’s value and a given number are equal.

### Number Validation

func NSDecimalIsNotANumber(UnsafePointer&lt;Decimal>) -> Bool

Returns a Boolean that indicates whether a given decimal contains a valid number.

### Initializers

init?(coder: NSCoder)

### Default Implementations

ExpressibleByBooleanLiteral Implementations

ExpressibleByFloatLiteral Implementations

ExpressibleByIntegerLiteral Implementations

## Relationships

### Inherits From

- NSValue

### Inherited By

- NSDecimalNumber

### Conforms To

- CKRecordValue
- CKRecordValueProtocol
- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- ExpressibleByBooleanLiteral
- ExpressibleByFloatLiteral
- ExpressibleByIntegerLiteral
- Hashable
- NSCoding
- NSCopying
- NSFetchRequestResult
- NSObjectProtocol
- NSSecureCoding
- Sendable

