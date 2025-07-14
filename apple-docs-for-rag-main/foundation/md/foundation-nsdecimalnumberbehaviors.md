

- Foundation
-  NSDecimalNumberBehaviors 

Protocol

# NSDecimalNumberBehaviors

A protocol that declares three methods that control the discretionary aspects of working with decimal numbers.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSDecimalNumberBehaviors
```

## Overview

The scale() and roundingMode() methods determine the precision of `NSDecimalNumber`’s return values and the way in which those values should be rounded to fit that precision. The exceptionDuringOperation(_:error:leftOperand:rightOperand:) method determines the way in which an `NSDecimalNumber` object should handle different calculation errors.

For an example of a class that adopts the `NSDecimalBehaviors` protocol, see the specification for NSDecimalNumberHandler.

## Topics

### Rounding

func roundingMode() -> NSDecimalNumber.RoundingMode

Returns the way that `NSDecimalNumber`’s `decimalNumberBy...` methods round their return values.

**Required**

func scale() -> Int16

Returns the number of digits allowed after the decimal separator.

**Required**

### Handling errors

func exceptionDuringOperation(Selector, error: NSDecimalNumber.CalculationError, leftOperand: NSDecimalNumber, rightOperand: NSDecimalNumber?) -> NSDecimalNumber?

Specifies what an `NSDecimalNumber` object will do when it encounters an error.

**Required**

### Constants

enum RoundingMode

These constants specify rounding behaviors.

enum CalculationError

Calculation error constants used to describe an error in exceptionDuringOperation(_:error:leftOperand:rightOperand:).

## Relationships

### Conforming Types

- NSDecimalNumberHandler

## See Also

### Managing Behavior

class var defaultBehavior: any NSDecimalNumberBehaviors

The way arithmetic methods round off and handle error conditions.

class NSDecimalNumberHandler

A class that adopts the decimal number behaviors protocol.

