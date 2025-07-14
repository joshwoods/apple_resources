

- Foundation
- MassFormatter
-  string(fromKilograms:) 

Instance Method

# string(fromKilograms:)

Returns a mass string for the provided value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func string(fromKilograms numberInKilograms: Double) -> String
```

## Parameters 

`numberInKilograms`  

The mass’s value in kilograms.

## Return Value

A string that combines a value and a unit string appropriate for the formatter’s locale.

## Discussion

This method converts the provided mass in kilograms into units appropriate for the formatter’s locale.

## See Also

### Formatting Mass Strings

var isForPersonMassUse: Bool

A Boolean value that indicates whether the resulting string represents a person’s mass.

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

This method is not supported for the `NSMassFormatter` class.

var numberFormatter: NumberFormatter!

The number formatter used to format the numbers in a mass strings.

func string(fromValue: Double, unit: MassFormatter.Unit) -> String

Returns a properly formatted mass string for the given value and unit.

func unitString(fromKilograms: Double, usedUnit: UnsafeMutablePointer&lt;MassFormatter.Unit>?) -> String

Returns the unit string for the provided value.

func unitString(fromValue: Double, unit: MassFormatter.Unit) -> String

Returns the unit string based on the provided value and unit.

var unitStyle: Formatter.UnitStyle

The unit style used by this formatter.

