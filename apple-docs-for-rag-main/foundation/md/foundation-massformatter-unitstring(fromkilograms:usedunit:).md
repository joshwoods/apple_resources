

- Foundation
- MassFormatter
-  unitString(fromKilograms:usedUnit:) 

Instance Method

# unitString(fromKilograms:usedUnit:)

Returns the unit string for the provided value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func unitString(
    fromKilograms numberInKilograms: Double,
    usedUnit unitp: UnsafeMutablePointer?
) -> String
```

## Parameters 

`numberInKilograms`  

The mass’s value in kilograms.

`unitp`  

An output parameter. This will hold the MassFormatter.Unit value that corresponds to the returned units.

## Return Value

A localized string representing the unit.

## Discussion

This method selects the correct unit based on the formatter’s locale, the magnitude of the value, and the isForPersonMassUse property. The value, once converted into the appropriate unit, determines whether the unit string is plural or singular.

## See Also

### Formatting Mass Strings

var isForPersonMassUse: Bool

A Boolean value that indicates whether the resulting string represents a person’s mass.

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

This method is not supported for the `NSMassFormatter` class.

var numberFormatter: NumberFormatter!

The number formatter used to format the numbers in a mass strings.

func string(fromKilograms: Double) -> String

Returns a mass string for the provided value.

func string(fromValue: Double, unit: MassFormatter.Unit) -> String

Returns a properly formatted mass string for the given value and unit.

func unitString(fromValue: Double, unit: MassFormatter.Unit) -> String

Returns the unit string based on the provided value and unit.

var unitStyle: Formatter.UnitStyle

The unit style used by this formatter.

