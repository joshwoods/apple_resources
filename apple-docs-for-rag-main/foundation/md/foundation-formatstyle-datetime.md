

- Foundation
- FormatStyle
-  dateTime 

Type Property

# dateTime

A style for formatting a date and time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var dateTime: Date.FormatStyle { get }
```

Available when `Self` is `Date.FormatStyle`.

## Discussion

Use this type property when the call point allows the use of Date.FormatStyle. You typically do this when calling the formatted(_:) method of Date.

Customize the date format style using modifier syntax to apply specific date and time formats. For example:

```
let meetingDate = Date()
let localeArray = ["en_US", "sv_SE", "en_GB", "th_TH", "fr_BE"]
let formattedDates = localeArray.map { localeID in
    meetingDate.formatted(.dateTime
                          .day(.twoDigits)
                          .month(.wide)
                          .weekday(.short)
                          .hour(.conversationalTwoDigits(amPM: .wide))
                          .locale(Locale(identifier: localeID)))
        } // ["Mo, July 31 at 05 PM", "må 31 juli 17", "Mo, 31 July at 17", "จ. 31 กรกฎาคม เวลา 17", "lu 31 juillet à 17 h"]
```

The default format styles provided are numeric date format and shortened time format. For example:

```
let meetingDate = Date()
let formatted = meetingDate.formatted(.dateTime) // "7/31/2023, 5:15 PM"
```

## See Also

### Applying date and time styles

struct FormatStyle

A structure that creates a locale-appropriate string representation of a date instance and converts strings of dates and times into date instances.

static var iso8601: Date.ISO8601FormatStyle

A style for formatting a date in accordance with the ISO-8601 standard.

struct ISO8601FormatStyle

A type that converts between dates and their ISO-8601 string representations.

static func verbatim(Date.FormatString, locale: Locale?, timeZone: TimeZone, calendar: Calendar) -> Date.VerbatimFormatStyle

Returns a style for formatting a date with an explicitly-specified style.

struct VerbatimFormatStyle

A style that formats a date with an explicitly-specified style.

static var interval: Date.IntervalFormatStyle

A style for formatting a date interval.

struct IntervalFormatStyle

A format style that creates string representations of date intervals.

static func relative(presentation: Date.RelativeFormatStyle.Presentation, unitsStyle: Date.RelativeFormatStyle.UnitsStyle) -> Self

Returns a style for formatting a date as relative to the current date.

struct RelativeFormatStyle

A format style that forms locale-aware string representations of a relative date or time.

static func components(style: Date.ComponentsFormatStyle.Style, fields: Set&lt;Date.ComponentsFormatStyle.Field>?) -> Self

Returns a style for formatting a date interval in terms of specific date components.

struct ComponentsFormatStyle

A style for formatting a date interval in terms of specific date components.

