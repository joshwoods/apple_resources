

- Foundation
- MassFormatter
-  isForPersonMassUse 

Instance Property

# isForPersonMassUse

A Boolean value that indicates whether the resulting string represents a person’s mass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isForPersonMassUse: Bool { get set }
```

## Discussion

Returns true if the value passed to string(fromKilograms:) or unitString(fromKilograms:usedUnit:) is a person’s mass; otherwise, false. By default, this property returns false.

The mass formatter uses this property when determining the best unit for a given locale (for example, in the string(fromKilograms:) method).

## See Also

### Formatting Mass Strings

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

This method is not supported for the `NSMassFormatter` class.

var numberFormatter: NumberFormatter!

The number formatter used to format the numbers in a mass strings.

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

