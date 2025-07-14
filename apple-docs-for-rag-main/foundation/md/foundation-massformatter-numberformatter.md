

- Foundation
- MassFormatter
-  numberFormatter 

Instance Property

# numberFormatter

The number formatter used to format the numbers in a mass strings.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var numberFormatter: NumberFormatter! { get set }
```

## Discussion

This property defaults to a number formatter using the NumberFormatter.Style.decimal style. You can provide a different number formatter to customize the mass string’s appearance.

## See Also

### Formatting Mass Strings

var isForPersonMassUse: Bool

A Boolean value that indicates whether the resulting string represents a person’s mass.

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

This method is not supported for the `NSMassFormatter` class.

func string(fromKilograms: Double) -> String

Returns a mass string for the provided value.

func string(fromValue: Double, unit: MassFormatter.Unit) -> String

Returns a properly formatted mass string for the given value and unit.

func unitString(fromKilograms: Double, usedUnit: UnsafeMutablePointer&lt;MassFormatter.Unit>?) -> String

Returns the unit string for the provided value.

func unitString(fromValue: Double, unit: MassFormatter.Unit) -> String

Returns the unit string based on the provided value and unit.

var unitStyle: Formatter.UnitStyle

The unit style used by this formatter.

