

- Foundation
- NSDecimalNumber
-  NSDecimalNumber.RoundingMode 

Enumeration

# NSDecimalNumber.RoundingMode

These constants specify rounding behaviors.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum RoundingMode
```

## Overview

The rounding mode matters only if the scale() method sets a limit on the precision of `NSDecimalNumber` return values. It has no effect if scale() returns `NSDecimalNoScale`. Assuming that scale() returns 1, the rounding mode has the following effects on various original values:

| Original Value | NSRoundPlain | NSRoundDown & NS RoundUp | NSRoundBankers |
|----------------|--------------|--------------------------|----------------|
| 1.24           | 1.2          | 1.2 & 1.3                | 1.2            |
| 1.26           | 1.3          | 1.2 & 1.3                | 1.3            |
| 1.25           | 1.3          | 1.2 & 1.3                | 1.2            |
| 1.35           | 1.4          | 1.3 & 1.4                | 1.4            |
| –1.35          | –1.4         | –1.4 & -1.3              | –1.4           |

## Topics

### Constants

case plain

Round to the closest possible return value; when caught halfway between two positive numbers, round up; when caught between two negative numbers, round down.

case down

Round return values down.

case up

Round return values up.

case bankers

Round to the closest possible return value; when halfway between two possibilities, return the possibility whose last digit is even.

case plain

Round to the closest possible return value; when caught halfway between two positive numbers, round up; when caught between two negative numbers, round down.

case down

Round return values down.

case up

Round return values up.

case bankers

Round to the closest possible return value; when halfway between two possibilities, return the possibility whose last digit is even.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Performing arithmetic using references

func NSDecimalCompact(UnsafeMutablePointer&lt;Decimal>)

Compacts the decimal structure for efficiency.

func NSDecimalAdd(UnsafeMutablePointer&lt;Decimal>, UnsafePointer&lt;Decimal>, UnsafePointer&lt;Decimal>, NSDecimalNumber.RoundingMode) -> NSDecimalNumber.CalculationError

Adds two decimal values.

func NSDecimalSubtract(UnsafeMutablePointer&lt;Decimal>, UnsafePointer&lt;Decimal>, UnsafePointer&lt;Decimal>, NSDecimalNumber.RoundingMode) -> NSDecimalNumber.CalculationError

Subtracts one decimal value from another.

func NSDecimalDivide(UnsafeMutablePointer&lt;Decimal>, UnsafePointer&lt;Decimal>, UnsafePointer&lt;Decimal>, NSDecimalNumber.RoundingMode) -> NSDecimalNumber.CalculationError

Divides one decimal value by another.

func NSDecimalMultiply(UnsafeMutablePointer&lt;Decimal>, UnsafePointer&lt;Decimal>, UnsafePointer&lt;Decimal>, NSDecimalNumber.RoundingMode) -> NSDecimalNumber.CalculationError

Multiplies two decimal numbers together.

func NSDecimalMultiplyByPowerOf10(UnsafeMutablePointer&lt;Decimal>, UnsafePointer&lt;Decimal>, Int16, NSDecimalNumber.RoundingMode) -> NSDecimalNumber.CalculationError

Multiplies a decimal by the specified power of 10.

func NSDecimalRound(UnsafeMutablePointer&lt;Decimal>, UnsafePointer&lt;Decimal>, Int, NSDecimalNumber.RoundingMode)

Rounds off the decimal value.

func NSDecimalPower(UnsafeMutablePointer&lt;Decimal>, UnsafePointer&lt;Decimal>, Int, NSDecimalNumber.RoundingMode) -> NSDecimalNumber.CalculationError

Raises the decimal value to the specified power.

func NSDecimalNormalize(UnsafeMutablePointer&lt;Decimal>, UnsafeMutablePointer&lt;Decimal>, NSDecimalNumber.RoundingMode) -> NSDecimalNumber.CalculationError

Normalizes the internal format of two decimal numbers to simplify later operations.

typealias RoundingMode

An alias for an enumeration that specifies possible rounding modes.

typealias CalculationError

An alias for a type that specifies possible calculation errors.

enum CalculationError

Calculation error constants used to describe an error in exceptionDuringOperation(_:error:leftOperand:rightOperand:).

