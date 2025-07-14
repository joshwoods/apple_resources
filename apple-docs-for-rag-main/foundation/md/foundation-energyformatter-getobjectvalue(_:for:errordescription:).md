

- Foundation
- EnergyFormatter
-  getObjectValue(\_:for:errorDescription:) 

Instance Method

# getObjectValue(\_:for:errorDescription:)

This method is not supported for the `NSEnergyFormatter` class.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getObjectValue(
    _ obj: AutoreleasingUnsafeMutablePointer?,
    for string: String,
    errorDescription error: AutoreleasingUnsafeMutablePointer?
) -> Bool
```

## Parameters 

`obj`  

An output parameter. If overridden, this parameter should contain the object created from the provided string.

`string`  

A string representation of the object.

`error`  

An output parameter. If overridden, this parameter should contain a description of any errors that occur. If you do not want to receive error messages, set this parameter to `NULL`.

## Return Value

true if the conversion from string was successful; otherwise, false.

## Discussion

You can override this method in a subclass. For more information, see Formatter.

## See Also

### Related Documentation

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

The default implementation of this method raises an exception.

### Formatting Energy Strings

var isForFoodEnergyUse: Bool

A Boolean value that indicates whether the energy value is used to measure food energy.

var numberFormatter: NumberFormatter!

The number formatter used to format the numbers in energy strings.

func string(fromJoules: Double) -> String

Returns an energy string for the provided value.

func string(fromValue: Double, unit: EnergyFormatter.Unit) -> String

Returns a properly formatted energy string for the given value and unit.

func unitString(fromJoules: Double, usedUnit: UnsafeMutablePointer&lt;EnergyFormatter.Unit>?) -> String

Returns the unit string for the provided value.

func unitString(fromValue: Double, unit: EnergyFormatter.Unit) -> String

Returns the unit string based on the provided value and unit.

var unitStyle: Formatter.UnitStyle

The unit style used by this formatter.

