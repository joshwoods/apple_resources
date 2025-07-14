

- Swift
- RegexComponent
-  iso8601WithTimeZone(includingFractionalSeconds:dateSeparator:dateTimeSeparator:timeSeparator:timeZoneSeparator:) 

Type Method

# iso8601WithTimeZone(includingFractionalSeconds:dateSeparator:dateTimeSeparator:timeSeparator:timeZoneSeparator:)

Creates a regex component that matches an ISO 8601-formatted date string that includes a time zone component, capturing the matched substring as a Foundation date.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func iso8601WithTimeZone(
    includingFractionalSeconds: Bool = false,
    dateSeparator: Date.ISO8601FormatStyle.DateSeparator = .dash,
    dateTimeSeparator: Date.ISO8601FormatStyle.DateTimeSeparator = .standard,
    timeSeparator: Date.ISO8601FormatStyle.TimeSeparator = .colon,
    timeZoneSeparator: Date.ISO8601FormatStyle.TimeZoneSeparator = .omitted
) -> Self
```

Available when `Self` is `Date.ISO8601FormatStyle`.

## Parameters 

`includingFractionalSeconds`  

A Boolean value that specifies whether the source string contains fractional seconds. The default is `false`.

`dateSeparator`  

The character that separates year, month, and day sections of the date substring. The default is Date.ISO8601FormatStyle.DateSeparator.dash.

`dateTimeSeparator`  

The character that separates the date and time sections of the substring. The default is Date.ISO8601FormatStyle.DateTimeSeparator.standard.

`timeSeparator`  

The character that separates the date and time sections of the substring. The default is Date.ISO8601FormatStyle.TimeSeparator.colon.

`timeZoneSeparator`  

The character that separates the hour, minute, and second sections of the substring. The default is Date.ISO8601FormatStyle.TimeSeparator.colon

## Return Value

A `RegexComponent` that matches ISO 8601-formatted date substrings as Foundation Date instances.

## Discussion

This method matches an ISO 8601 date string using the provided separator characters.

The following example creates a Regex that matches an ISO 8601-formatted date. The format looks for a dash for the date separator, the standard date/time separator (none), a colon for the time separator, and no separator for the time zone. It then matches this regex against a source string containing a date with this format (specifying a time zone five hours behind UTC), some whitespace, a substring, more whitespace, and a currency value.

```
let iso860Source = "2022-07-14T21:10:15-05:00   Lemon-lime slushie      $1.99"
let matcher = Regex {
    Capture {
        One(.iso8601WithTimeZone(includingFractionalSeconds: false,
                                 dateSeparator: .dash,
                                 dateTimeSeparator: .standard,
                                 timeSeparator: .colon,
                                 timeZoneSeparator: .omitted))
    }
    OneOrMore(.horizontalWhitespace)
    OneOrMore(.any)
    OneOrMore(.horizontalWhitespace)
    One(.localizedCurrency(code:Locale.Currency("USD"),
                           locale:Locale(identifier: "en_US")))
}
let match = iso860Source.firstMatch(of: matcher)
let date = match?.1 // date == Jul 14, 2022 at 7:10 PM (may vary depending on current locale)
```

## See Also

### Matching dates and times

static func date(Date.FormatStyle.DateStyle, locale: Locale, timeZone: TimeZone, calendar: Calendar?) -> Date.ParseStrategy

Creates a regex component that matches a localized date string formatted in accordance with a style, capturing it as a Foundation date.

static func date(format: Date.FormatString, locale: Locale, timeZone: TimeZone, calendar: Calendar?, twoDigitStartDate: Date) -> Self

Creates a regex component that matches a localized date string formatted in accordance with a format string, capturing it as a Foundation date.

static func dateTime(date: Date.FormatStyle.DateStyle, time: Date.FormatStyle.TimeStyle, locale: Locale, timeZone: TimeZone, calendar: Calendar?) -> Date.ParseStrategy

Creates a regex component that matches a localized date and time string, capturing it as a Foundation date.

static var iso8601: Date.ISO8601FormatStyle

A regex component that matches a default ISO 8601-formatted date string, capturing it as a Foundation date.

static func iso8601Date(timeZone: TimeZone, dateSeparator: Date.ISO8601FormatStyle.DateSeparator) -> Self

Creates a regex component that matches an ISO 8601-formatted date string, capturing it as a Foundation date in the specified time zone.

static func iso8601(timeZone: TimeZone, includingFractionalSeconds: Bool, dateSeparator: Date.ISO8601FormatStyle.DateSeparator, dateTimeSeparator: Date.ISO8601FormatStyle.DateTimeSeparator, timeSeparator: Date.ISO8601FormatStyle.TimeSeparator) -> Self

Creates a regex component that matches an ISO 8601-formatted date string, capturing the matched substring as a Foundation date in the specified time zone.

