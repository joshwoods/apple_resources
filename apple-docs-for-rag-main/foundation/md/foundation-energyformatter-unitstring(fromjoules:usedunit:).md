

- Foundation
- EnergyFormatter
-  unitString(fromJoules:usedUnit:) 

Instance Method

# unitString(fromJoules:usedUnit:)

Returns the unit string for the provided value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func unitString(
    fromJoules numberInJoules: Double,
    usedUnit unitp: UnsafeMutablePointer?
) -> String
```

## Parameters 

`numberInJoules`  

The energy value in joules.

`unitp`  

An output parameter. This will hold the EnergyFormatter.Unit value that corresponds to the returned units.

## Return Value

A localized string representing the unit.

## Discussion

This method selects the correct unit based on the formatter’s locale, the magnitude of the value, and the isForFoodEnergyUse property.

## See Also

### Formatting Energy Strings

var isForFoodEnergyUse: Bool

A Boolean value that indicates whether the energy value is used to measure food energy.

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

This method is not supported for the `NSEnergyFormatter` class.

var numberFormatter: NumberFormatter!

The number formatter used to format the numbers in energy strings.

func string(fromJoules: Double) -> String

Returns an energy string for the provided value.

func string(fromValue: Double, unit: EnergyFormatter.Unit) -> String

Returns a properly formatted energy string for the given value and unit.

func unitString(fromValue: Double, unit: EnergyFormatter.Unit) -> String

Returns the unit string based on the provided value and unit.

var unitStyle: Formatter.UnitStyle

The unit style used by this formatter.

