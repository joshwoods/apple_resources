

- Foundation
- DateComponentsFormatter
-  unitsStyle 

Instance Property

# unitsStyle

The formatting style for unit names.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var unitsStyle: DateComponentsFormatter.UnitsStyle { get set }
```

## Discussion

Configures the strings to use (if any) for unit names such as days, hours, minutes, and seconds. Use this property to specify whether you want abbreviated or shortened versions of unit names—for example, `hrs` instead of `hours`.

The default value of this property is DateComponentsFormatter.UnitsStyle.positional.

## See Also

### Configuring the Formatter Options

var allowedUnits: NSCalendar.Unit

The bitmask of calendrical units such as day and month to include in the output string.

var allowsFractionalUnits: Bool

A Boolean indicating whether non-integer units may be used for values.

var calendar: Calendar?

The default calendar to use when formatting date components.

var collapsesLargestUnit: Bool

A Boolean value indicating whether to collapse the largest unit into smaller units when a certain threshold is met.

var includesApproximationPhrase: Bool

A Boolean value indicating whether the resulting phrase reflects an inexact time value.

var includesTimeRemainingPhrase: Bool

A Boolean value indicating whether output strings reflect the amount of time remaining.

var maximumUnitCount: Int

The maximum number of time units to include in the output string.

var zeroFormattingBehavior: DateComponentsFormatter.ZeroFormattingBehavior

The formatting style for units whose value is 0.

