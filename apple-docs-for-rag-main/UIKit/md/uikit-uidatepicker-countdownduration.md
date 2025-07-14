

- UIKit
- UIDatePicker
-  countDownDuration 

Instance Property

# countDownDuration

The value displayed by the date picker when the mode property is set to show a countdown time.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var countDownDuration: TimeInterval { get set }
```

## Discussion

Use this property to get and set the currently selected value when the date picker’s mode property is set to UIDatePicker.Mode.countDownTimer. This property is of type TimeInterval and therefore is measured in seconds, although the date picker displays only hours and minutes. If the mode of the date picker is not UIDatePicker.Mode.countDownTimer, this value is undefined; refer instead to the date property. The default value is 0.0 and the maximum value is 23:59 (86,340 seconds).

## See Also

### Configuring temporal attributes

var maximumDate: Date?

The maximum date that a date picker can show.

var minimumDate: Date?

The minimum date that a date picker can show.

var minuteInterval: Int

The interval at which the date picker should display minutes.

var roundsToMinuteInterval: Bool

A Boolean value that determines whether the date rounds to a specific minute interval.

