

- Foundation
- DateComponentsFormatter
-  calendar 

Instance Property

# calendar

The default calendar to use when formatting date components.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var calendar: Calendar? { get set }
```

## Discussion

The formatter uses the calendar in this property to format values that do not have an inherent calendar of their own. For example, the formatter uses this calendar when formatting an TimeInterval value.

The default value of this property is the calendar returned by the autoupdatingCurrent method of NSCalendar. Setting this property to `nil` causes the formatter to use the Gregorian calendar with the `en_US_POSIX` locale.

## See Also

### Configuring the Formatter Options

var allowedUnits: NSCalendar.Unit

The bitmask of calendrical units such as day and month to include in the output string.

var allowsFractionalUnits: Bool

A Boolean indicating whether non-integer units may be used for values.

var collapsesLargestUnit: Bool

A Boolean value indicating whether to collapse the largest unit into smaller units when a certain threshold is met.

var includesApproximationPhrase: Bool

A Boolean value indicating whether the resulting phrase reflects an inexact time value.

var includesTimeRemainingPhrase: Bool

A Boolean value indicating whether output strings reflect the amount of time remaining.

var maximumUnitCount: Int

The maximum number of time units to include in the output string.

var unitsStyle: DateComponentsFormatter.UnitsStyle

The formatting style for unit names.

var zeroFormattingBehavior: DateComponentsFormatter.ZeroFormattingBehavior

The formatting style for units whose value is 0.

