

- UIKit
- UIDatePicker
-  minuteInterval 

Instance Property

# minuteInterval

The interval at which the date picker should display minutes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var minuteInterval: Int { get set }
```

## Discussion

Use this property to set the interval displayed by the minutes wheel (for example, 15 minutes). The interval value must be evenly divided into 60; if it isn’t, the default value is used. The default and minimum values are 1; the maximum value is 30.

## See Also

### Configuring temporal attributes

var maximumDate: Date?

The maximum date that a date picker can show.

var minimumDate: Date?

The minimum date that a date picker can show.

var countDownDuration: TimeInterval

The value displayed by the date picker when the mode property is set to show a countdown time.

var roundsToMinuteInterval: Bool

A Boolean value that determines whether the date rounds to a specific minute interval.

