

- UIKit
- UIDatePicker
-  roundsToMinuteInterval 

Instance Property

# roundsToMinuteInterval

A Boolean value that determines whether the date rounds to a specific minute interval.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var roundsToMinuteInterval: Bool { get set }
```

## Discussion

If this property is true, date always rounds to the minuteInterval and only produces dates that align with the minute interval. If this property is false, changes to date ignore the minuteInterval property.

The default value is true.

## See Also

### Configuring temporal attributes

var maximumDate: Date?

The maximum date that a date picker can show.

var minimumDate: Date?

The minimum date that a date picker can show.

var minuteInterval: Int

The interval at which the date picker should display minutes.

var countDownDuration: TimeInterval

The value displayed by the date picker when the mode property is set to show a countdown time.

