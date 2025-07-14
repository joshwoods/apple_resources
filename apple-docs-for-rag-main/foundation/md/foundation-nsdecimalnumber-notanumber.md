

- Foundation
- NSDecimalNumber
-  notANumber 

Type Property

# notANumber

A decimal number that specifies no number.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
class var notANumber: NSDecimalNumber { get }
```

## Return Value

An `NSDecimalNumber` object that specifies no number.

## Discussion

Any arithmetic method receiving notANumber as an argument returns notANumber.

This value can be a useful way of handling non-numeric data in an input file. This method can also be a useful response to calculation errors. For more information on calculation errors, see the exceptionDuringOperation(_:error:leftOperand:rightOperand:) method description in the NSDecimalNumberBehaviors protocol specification.

## See Also

### Creating a Decimal Number

class var one: NSDecimalNumber

A decimal number equivalent to the number 1.0.

class var zero: NSDecimalNumber

A decimal number equivalent to the number 0.0.

