

- Foundation
- LengthFormatter
-  numberFormatter 

Instance Property

# numberFormatter

The number formatter used to format the numbers in length strings.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var numberFormatter: NumberFormatter! { get set }
```

## Discussion

This property defaults to a number formatter using the NumberFormatter.Style.decimal. You can provide a different number formatter to customize the length string’s appearance.

## See Also

### Formatting Length Strings

var isForPersonHeightUse: Bool

A Boolean value that indicates whether the resulting string represents a person’s height.

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

This method is not supported for the `NSLengthFormatter` class.

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

