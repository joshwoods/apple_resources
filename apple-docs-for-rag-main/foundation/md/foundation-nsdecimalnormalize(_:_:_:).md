

- Foundation
-  NSDecimalNormalize(\_:\_:\_:) 

Function

# NSDecimalNormalize(\_:\_:\_:)

Normalizes the internal format of two decimal numbers to simplify later operations.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSDecimalNormalize(
    _ number1: UnsafeMutablePointer,
    _ number2: UnsafeMutablePointer,
    _ roundingMode: NSDecimalNumber.RoundingMode
) -> NSDecimalNumber.CalculationError
```

## Discussion

Decimal instances are represented in memory as a mantissa and an exponent, expressing the value mantissa x 10^exponent. A number can have many representations; for example, the following table lists several valid representations for the number 100:

| Mantissa | Exponent |
|----------|----------|
| 100      | 0        |
| 10       | 1        |
| 1        | 2        |

Format `number1` and `number2` so that they have equal exponents. This format makes addition and subtraction very convenient. Both NSDecimalAdd(_:_:_:_:) and NSDecimalSubtract(_:_:_:_:) call NSDecimalNormalize(_:_:_:). You may want to use it if you write more complicated addition or subtraction routines.

For explanations of the possible return values, see NSDecimalAdd(_:_:_:_:).

For more information, see Number and Value Programming Topics.

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

typealias RoundingMode

An alias for an enumeration that specifies possible rounding modes.

enum RoundingMode

These constants specify rounding behaviors.

typealias CalculationError

An alias for a type that specifies possible calculation errors.

enum CalculationError

Calculation error constants used to describe an error in exceptionDuringOperation(_:error:leftOperand:rightOperand:).

