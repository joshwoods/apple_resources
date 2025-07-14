

- UIKit
- UIDatePicker
-  locale 

Instance Property

# locale

The locale used by the date picker.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var locale: Locale? { get set }
```

## Discussion

The default value is the current locale as returned by the current property of NSLocale, or the locale used by the date picker’s calendar. Locales encapsulate information about facets of a language or culture, such as the way dates are formatted.

## See Also

### Managing the date and calendar

var calendar: Calendar!

The calendar to use for the date picker.

var date: Date

The date displayed by the date picker.

func setDate(Date, animated: Bool)

Sets the date to display in the date picker, with an option to animate the setting.

var timeZone: TimeZone?

The time zone reflected in the date displayed by the date picker.

