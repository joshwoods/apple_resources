

- Foundation
-  NSDecimalAdd(\_:\_:\_:\_:) 

Function

# NSDecimalAdd(\_:\_:\_:\_:)

Adds two decimal values.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSDecimalAdd(
    _ result: UnsafeMutablePointer,
    _ leftOperand: UnsafePointer,
    _ rightOperand: UnsafePointer,
    _ roundingMode: NSDecimalNumber.RoundingMode
) -> NSDecimalNumber.CalculationError
```

## Discussion

Adds `leftOperand` to `rightOperand` and stores the sum in `result`. Decimal instances can represent a number with up to 38 significant digits. If a number is more precise than that, it must be rounded off. `roundingMode` determines how to round it off. There are four possible rounding modes:

- NSDecimalNumber.RoundingMode.down

- NSDecimalNumber.RoundingMode.up

- NSDecimalNumber.RoundingMode.plain

- NSDecimalNumber.RoundingMode.bankers

The return value indicates whether any machine limitations were encountered in the addition. If none were encountered, the function returns `NSCalculationNoError`. Otherwise it may return one of the following values: `NSCalculationLossOfPrecision`, `NSCalculationOverflow` or `NSCalculationUnderflow`. For descriptions of all these error conditions, see exceptionDuringOperation(_:error:leftOperand:rightOperand:) in NSDecimalNumberBehaviors.

For more information, see Number and Value Programming Topics.

## See Also

### Performing arithmetic using references

func NSDecimalCompact(UnsafeMutablePointer&lt;Decimal>)

Compacts the decimal structure for efficiency.

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

enum RoundingMode

These constants specify rounding behaviors.

typealias CalculationError

An alias for a type that specifies possible calculation errors.

enum CalculationError

Calculation error constants used to describe an error in exceptionDuringOperation(_:error:leftOperand:rightOperand:).

