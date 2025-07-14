

- Foundation
-  NSDecimalMultiplyByPowerOf10(\_:\_:\_:\_:) 

Function

# NSDecimalMultiplyByPowerOf10(\_:\_:\_:\_:)

Multiplies a decimal by the specified power of 10.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSDecimalMultiplyByPowerOf10(
    _ result: UnsafeMutablePointer,
    _ number: UnsafePointer,
    _ power: Int16,
    _ roundingMode: NSDecimalNumber.RoundingMode
) -> NSDecimalNumber.CalculationError
```

## Discussion

Multiplies `number` by `power` of 10 and stores the product, possibly rounded off according to `roundingMode`, in `result`.

For explanations of the possible return values and rounding modes, see NSDecimalAdd(_:_:_:_:).

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

