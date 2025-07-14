

- Foundation
- LengthFormatter
-  isForPersonHeightUse 

Instance Property

# isForPersonHeightUse

A Boolean value that indicates whether the resulting string represents a person’s height.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isForPersonHeightUse: Bool { get set }
```

## Discussion

Returns true if the value passed to string(fromMeters:) or unitString(fromMeters:usedUnit:) is a person’s height; otherwise, false. By default, this property returns false.

The length formatter uses this property when determining the best unit for a given locale (for example, in the string(fromMeters:) method).

## See Also

### Formatting Length Strings

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

This method is not supported for the `NSLengthFormatter` class.

var numberFormatter: NumberFormatter!

The number formatter used to format the numbers in length strings.

func string(fromMeters: Double) -> String

Returns a length string for the provided value.

func string(fromValue: Double, unit: LengthFormatter.Unit) -> String

Returns a properly formatted length string for the given value and unit.

func unitString(fromMeters: Double, usedUnit: UnsafeMutablePointer&lt;LengthFormatter.Unit>?) -> String

Returns the unit string for the provided value.

func unitString(fromValue: Double, unit: LengthFormatter.Unit) -> String

Returns the unit string based on the provided value and unit.

var unitStyle: Formatter.UnitStyle

The unit style used by this formatter.

