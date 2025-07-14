

- Foundation
- DateComponentsFormatter
-  allowedUnits 

Instance Property

# allowedUnits

The bitmask of calendrical units such as day and month to include in the output string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var allowedUnits: NSCalendar.Unit { get set }
```

## Discussion

The allowed calendar units are:

- year

- month

- weekOfMonth

- day

- hour

- minute

- second

Assigning any other calendar units to this property results in an exception.

## See Also

### Configuring the Formatter Options

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

var unitsStyle: DateComponentsFormatter.UnitsStyle

The formatting style for unit names.

var zeroFormattingBehavior: DateComponentsFormatter.ZeroFormattingBehavior

The formatting style for units whose value is 0.

