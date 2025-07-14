

- Foundation
- DateComponentsFormatter
-  collapsesLargestUnit 

Instance Property

# collapsesLargestUnit

A Boolean value indicating whether to collapse the largest unit into smaller units when a certain threshold is met.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var collapsesLargestUnit: Bool { get set }
```

## Discussion

An example of when this property might apply is when expressing 63 seconds worth of time. When this property is set to true, the formatted value would be “63s”. When the value of this property is false, the formatted value would be “1m 3s”.

The default value of this property is false.

## See Also

### Configuring the Formatter Options

var allowedUnits: NSCalendar.Unit

The bitmask of calendrical units such as day and month to include in the output string.

var allowsFractionalUnits: Bool

A Boolean indicating whether non-integer units may be used for values.

var calendar: Calendar?

The default calendar to use when formatting date components.

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

