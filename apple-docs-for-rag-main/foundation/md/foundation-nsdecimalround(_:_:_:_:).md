

- Foundation
-  NSDecimalRound(\_:\_:\_:\_:) 

Function

# NSDecimalRound(\_:\_:\_:\_:)

Rounds off the decimal value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSDecimalRound(
    _ result: UnsafeMutablePointer,
    _ number: UnsafePointer,
    _ scale: Int,
    _ roundingMode: NSDecimalNumber.RoundingMode
)
```

## Discussion

Rounds `number` off according to the parameters `scale` and `roundingMode` and stores the result in `result`.

The `scale` value specifies the number of digits `result` can have after its decimal point. `roundingMode` specifies the way that number is rounded off. There are four possible values for `roundingMode`: NSDecimalNumber.RoundingMode.down, NSDecimalNumber.RoundingMode.up, NSDecimalNumber.RoundingMode.plain, and NSDecimalNumber.RoundingMode.bankers. For thorough discussions of `scale` and `roundingMode`, see NSDecimalNumberBehaviors.

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

