

- Foundation
- LengthFormatter
-  string(fromValue:unit:) 

Instance Method

# string(fromValue:unit:)

Returns a properly formatted length string for the given value and unit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func string(
    fromValue value: Double,
    unit: LengthFormatter.Unit
) -> String
```

## Parameters 

`value`  

The length’s value in the given unit.

`unit`  

The unit used in the resulting length string.

## Return Value

A localized string that combines the provided value and unit.

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

func unitString(fromMeters: Double, usedUnit: UnsafeMutablePointer&lt;LengthFormatter.Unit>?) -> String

Returns the unit string for the provided value.

func unitString(fromValue: Double, unit: LengthFormatter.Unit) -> String

Returns the unit string based on the provided value and unit.

var unitStyle: Formatter.UnitStyle

The unit style used by this formatter.

