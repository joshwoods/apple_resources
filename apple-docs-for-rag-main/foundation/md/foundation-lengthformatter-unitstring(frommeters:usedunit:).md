

- Foundation
- LengthFormatter
-  unitString(fromMeters:usedUnit:) 

Instance Method

# unitString(fromMeters:usedUnit:)

Returns the unit string for the provided value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func unitString(
    fromMeters numberInMeters: Double,
    usedUnit unitp: UnsafeMutablePointer?
) -> String
```

## Parameters 

`numberInMeters`  

The length’s value in meters.

`unitp`  

An output parameter. This will hold the LengthFormatter.Unit value that corresponds to the returned units.

## Return Value

A localized string representing the unit.

## Discussion

This method selects the correct unit based on the formatter’s locale, the magnitude of the value, and the isForPersonHeightUse property.

## See Also

### Formatting Length Strings

var isForPersonHeightUse: Bool

A Boolean value that indicates whether the resulting string represents a person’s height.

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

This method is not supported for the `NSLengthFormatter` class.

var numberFormatter: NumberFormatter!

The number formatter used to format the numbers in length strings.

func string(fromMeters: Double) -> String

Returns a length string for the provided value.

func string(fromValue: Double, unit: LengthFormatter.Unit) -> String

Returns a properly formatted length string for the given value and unit.

func unitString(fromValue: Double, unit: LengthFormatter.Unit) -> String

Returns the unit string based on the provided value and unit.

var unitStyle: Formatter.UnitStyle

The unit style used by this formatter.

