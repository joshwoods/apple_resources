

- Foundation
-  NSDecimalNumber 

Class

# NSDecimalNumber

An object for representing and performing arithmetic on base-10 numbers.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSDecimalNumber
```

## Overview

In Swift, this object bridges to Decimal; use NSDecimalNumber when you need reference semantics or other Foundation-specific behavior.

`NSDecimalNumber`, an immutable subclass of `NSNumber`, provides an object-oriented wrapper for doing base-10 arithmetic. An instance can represent any number that can be expressed as `mantissa x 10^exponent` where mantissa is a decimal integer up to 38 digits long, and exponent is an integer from –128 through 127.

Important

The Swift overlay to the Foundation framework provides the Decimal structure, which bridges to the NSDecimalNumber class. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Creating a Decimal Number

class var one: NSDecimalNumber

A decimal number equivalent to the number 1.0.

class var zero: NSDecimalNumber

A decimal number equivalent to the number 0.0.

class var notANumber: NSDecimalNumber

A decimal number that specifies no number.

### Initializing a Decimal Number

init(decimal: Decimal)

Initializes a decimal number to represent a given decimal.

convenience init(mantissa: UInt64, exponent: Int16, isNegative: Bool)

Initializes a decimal number using the given mantissa, exponent, and sign.

convenience init(string: String?)

Initializes a decimal number so that its value is equivalent to that in a given numeric string.

convenience init(string: String?, locale: Any?)

Initializes a decimal number so that its value is equivalent to that in a given numeric string, interpreted using a given locale.

### Performing Arithmetic

func adding(NSDecimalNumber) -> NSDecimalNumber

Adds this number to another given number.

func subtracting(NSDecimalNumber) -> NSDecimalNumber

Subtracts another given number from this one.

func multiplying(by: NSDecimalNumber) -> NSDecimalNumber

Multiplies the number by another given number.

func dividing(by: NSDecimalNumber) -> NSDecimalNumber

Divides the number by another given number.

func raising(toPower: Int) -> NSDecimalNumber

Raises the number to a given power.

func multiplying(byPowerOf10: Int16) -> NSDecimalNumber

Multiplies the number by 10 raised to the given power.

func adding(NSDecimalNumber, withBehavior: (any NSDecimalNumberBehaviors)?) -> NSDecimalNumber

Adds this number to another given number using the specified behavior.

func subtracting(NSDecimalNumber, withBehavior: (any NSDecimalNumberBehaviors)?) -> NSDecimalNumber

Subtracts this a given number from this one using the specified behavior.

func multiplying(by: NSDecimalNumber, withBehavior: (any NSDecimalNumberBehaviors)?) -> NSDecimalNumber

Multiplies this number by another given number using the specified behavior.

func dividing(by: NSDecimalNumber, withBehavior: (any NSDecimalNumberBehaviors)?) -> NSDecimalNumber

Divides this number by another given number using the specified behavior.

func raising(toPower: Int, withBehavior: (any NSDecimalNumberBehaviors)?) -> NSDecimalNumber

Raises the number to a given power using the specified behavior.

func multiplying(byPowerOf10: Int16, withBehavior: (any NSDecimalNumberBehaviors)?) -> NSDecimalNumber

Multiplies the number by 10 raised to the given power using the specified behavior.

### Rounding Off

func rounding(accordingToBehavior: (any NSDecimalNumberBehaviors)?) -> NSDecimalNumber

Returns a rounded version of the decimal number using the specified rounding behavior.

### Managing Behavior

class var defaultBehavior: any NSDecimalNumberBehaviors

The way arithmetic methods round off and handle error conditions.

protocol NSDecimalNumberBehaviors

A protocol that declares three methods that control the discretionary aspects of working with decimal numbers.

class NSDecimalNumberHandler

A class that adopts the decimal number behaviors protocol.

### Accessing the Value

var decimalValue: Decimal

The decimal number’s value, expressed as an Decimal structure.

var doubleValue: Double

The decimal number’s closest approximate `double` value.

func description(withLocale: Any?) -> String

var objCType: UnsafePointer&lt;CChar>

A C string containing the Objective-C type for the data contained in the decimal number object.

### Comparing Decimal Numbers

func compare(NSNumber) -> ComparisonResult

Compares this decimal number and another.

### Getting Maximum and Minimum Possible Values

class var maximum: NSDecimalNumber

Returns the largest possible value of a decimal number.

class var minimum: NSDecimalNumber

Returns the smallest possible value of a decimal number.

### Recognizing Exceptions

Exceptions with these names may be raised to indicate computational errors with decimal numbers.

static let decimalNumberExactnessException: NSExceptionName

The exception raised if there is an exactness error.

static let decimalNumberOverflowException: NSExceptionName

The exception raised on overflow.

static let decimalNumberUnderflowException: NSExceptionName

The exception raised on underflow.

static let decimalNumberDivideByZeroException: NSExceptionName

The exception raised on divide by zero.

## Relationships

### Inherits From

- NSNumber

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- ExpressibleByBooleanLiteral
- ExpressibleByFloatLiteral
- ExpressibleByIntegerLiteral
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

