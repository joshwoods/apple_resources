

- Foundation
- DateComponentsFormatter
-  maximumUnitCount 

Instance Property

# maximumUnitCount

The maximum number of time units to include in the output string.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var maximumUnitCount: Int { get set }
```

## Discussion

Use this property to limit the number of units displayed in the resulting string. For example, with this property set to 2, instead of “1h 10m, 30s”, the resulting string would be “1h 10m”. Use this property when you are constrained for space or want to round up values to the nearest large unit.

The default value of this property is `0`, which does not cause the elimination of any units.

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

var unitsStyle: DateComponentsFormatter.UnitsStyle

The formatting style for unit names.

var zeroFormattingBehavior: DateComponentsFormatter.ZeroFormattingBehavior

The formatting style for units whose value is 0.

