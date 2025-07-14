

- UIKit
- UIDatePicker
-  calendar 

Instance Property

# calendar

The calendar to use for the date picker.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var calendar: Calendar! { get set }
```

## Discussion

The default value of this property corresponds to the user’s current calendar as configured in Settings. This is equivalent to the value returned by calling the NSCalendar class method current. Setting this property to `nil` is equivalent to setting it to its default value.

Calendars specify the details of cultural systems used for reckoning time; they identify the beginning, length, and divisions of a year.

## See Also

### Managing the date and calendar

var date: Date

The date displayed by the date picker.

var locale: Locale?

The locale used by the date picker.

func setDate(Date, animated: Bool)

Sets the date to display in the date picker, with an option to animate the setting.

var timeZone: TimeZone?

The time zone reflected in the date displayed by the date picker.

