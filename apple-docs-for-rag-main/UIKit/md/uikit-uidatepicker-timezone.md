

- UIKit
- UIDatePicker
-  timeZone 

Instance Property

# timeZone

The time zone reflected in the date displayed by the date picker.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var timeZone: TimeZone? { get set }
```

## Discussion

The default value is `nil`, which tells the date picker to use the current time zone as returned by local (NSTimeZone) or the time zone used by the date picker’s calendar.

## See Also

### Managing the date and calendar

var calendar: Calendar!

The calendar to use for the date picker.

var date: Date

The date displayed by the date picker.

var locale: Locale?

The locale used by the date picker.

func setDate(Date, animated: Bool)

Sets the date to display in the date picker, with an option to animate the setting.

