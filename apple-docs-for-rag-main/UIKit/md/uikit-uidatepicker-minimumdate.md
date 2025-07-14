

- UIKit
- UIDatePicker
-  minimumDate 

Instance Property

# minimumDate

The minimum date that a date picker can show.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var minimumDate: Date? { get set }
```

## Discussion

Use this property to configure the minimum date that’s selected in the date picker interface. The property contains an NSDate object or `nil` (the default), which means no minimum date. This property, along with the maximumDate property, lets you specify a valid date range. If the minimum date value is greater than the maximum date value, both properties are ignored. The minimum and maximum dates are also ignored in the countdown-timer mode (UIDatePicker.Mode.countDownTimer).

## See Also

### Configuring temporal attributes

var maximumDate: Date?

The maximum date that a date picker can show.

var minuteInterval: Int

The interval at which the date picker should display minutes.

var countDownDuration: TimeInterval

The value displayed by the date picker when the mode property is set to show a countdown time.

var roundsToMinuteInterval: Bool

A Boolean value that determines whether the date rounds to a specific minute interval.

