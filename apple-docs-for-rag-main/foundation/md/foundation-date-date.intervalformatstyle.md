

- Foundation
- Date
-  Date.IntervalFormatStyle 

Structure

# Date.IntervalFormatStyle

A format style that creates string representations of date intervals.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct IntervalFormatStyle
```

## Overview

Use a date interval format style to create user-readable strings in the form of ` - ` for your app’s interface, where `` and `` are date values that you supply. The format style uses locale and language information, along with custom formatting options, to define the content of the resulting string.

`Date.IntervalFormatStyle` provides a variety of localized presets and configuration options to create user-visible representations of date intervals. When displaying a date interval to a user, use the formatted(date:time:) instance method of `Range`. Set the date and time styles of the date interval format style separately, according to your particular needs.

For example, to create a date interval string with a full date and no time representation, set the Date.IntervalFormatStyle.DateStyle to complete and the Date.IntervalFormatStyle.TimeStyle to omitted. The following example creates a formatted interval string with this style:

```
if let today = Calendar.current.date(byAdding: .day, value: -120, to: Date()),
    let thirtyDaysBeforeToday = Calendar.current.date(byAdding: .day, value: -30, to: today) {
    // today: June 5, 2023
    // thirtyDaysBeforeToday: May 6, 2023

    // Create a Range.
    let last30days = thirtyDaysBeforeToday..

You can create string representations of date intervals with various levels of brevity using a variety of preset date and time styles. The following example shows date styles of long, abbreviated, and numeric, and time styles of shortened, standard, and complete:

```
if let today = Calendar.current.date(byAdding: .day, value: -120, to: Date()),
   let thirtyDaysBeforeToday = Calendar.current.date(byAdding: .day, value: -30, to: today) {
   // today: Mar 1, 2021 at 8:01 PM
   // thirtyDaysBeforeToday: Jan 30, 2021 at 8:01 PM

   // Create a Range.
   let last30days = thirtyDaysBeforeToday..

The default date style is abbreviated and the default time style is shortened.

For full customization of the string representation of a date interval, use the formatted(_:) instance method of `Range` and provide a Date.IntervalFormatStyle instance.

You can achieve any customization of date and time representation your app requires by appying a series of convenience modifiers to your format style. The following example applies a series of modifiers to the format style to precisely define the formatting of the year, month, day, hour, minute, and time zone components of the resulting string:

```
if let today = Calendar.current.date(byAdding: .day, value: -140, to: Date()),
   let sevenDaysAfterToday = Calendar.current.date(byAdding: .day, value: 7, to: today) {

    // Create a Range.
    let weekFromNow = today.. and pass in an instance of Date.IntervalFormatStyle.
    weekFromNow.formatted(
        Date.IntervalFormatStyle()
            .year()
            .month(.abbreviated)
            .day()
            .hour(.defaultDigits(amPM: .narrow))
            .weekday(.abbreviated)
    ) //  Wed, Feb 10, 2021, 3 p – Wed, Feb 17, 2021, 3 p
}
```

Date.IntervalFormatStyle provides a convenient factory variable, `interval`, to shorten the syntax when applying date and time modifiers to customize the format.

```
if let today = Calendar.current.date(byAdding: .day, value: -140, to: Date()),
   let sevenDaysBeforeToday = Calendar.current.date(byAdding: .day, value: -7, to: today) {

    // Create a Range.
    let weekBefore = sevenDaysBeforeToday.. and pass in an instance of Date.IntervalFormatStyle.
        print(weekBefore.formatted(.interval
                 .day()
                 .month(.wide)
                 .weekday(.short)
                 .hour(.conversationalTwoDigits(amPM: .wide))
                 .locale(Locale(identifier: localeID))))
    }
}
// We, February 3, 3 PM – We, February 10, 3 PM
// on 3 februari 15 – on 10 februari 15
// We 3 February, 15 – We 10 February, 15
// พ. 3 กุมภาพันธ์ 15 – พ. 10 กุมภาพันธ์ 15
// me 3 février, 15 h – me 10 février, 15 h

```

## Topics

### Creating a Date Interval Format Style

init(date: Date.IntervalFormatStyle.DateStyle?, time: Date.IntervalFormatStyle.TimeStyle?, locale: Locale, calendar: Calendar, timeZone: TimeZone)

Creates an instance using the provided date, time, locale, calendar, time zone, and capitalization context.

### Specifying Date Interval Format Styles

func timeZone(Date.IntervalFormatStyle.Symbol.TimeZone) -> Date.IntervalFormatStyle

Modifies the date interval format style to use the specified time zone format.

var calendar: Calendar

The calendar for formatting the date interval.

var locale: Locale

The locale for formatting the date and time interval components.

var timeZone: TimeZone

The time zone for formatting the date interval components.

### Modifying Date Interval Format Styles

func day() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the day.

func hour(Date.IntervalFormatStyle.Symbol.Hour) -> Date.IntervalFormatStyle

Modifies the date interval format style to use the specified hour format style.

func minute() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the minutes.

func month(Date.IntervalFormatStyle.Symbol.Month) -> Date.IntervalFormatStyle

Modifies the date interval format style to include the month.

func second() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the seconds.

func weekday(Date.IntervalFormatStyle.Symbol.Weekday) -> Date.IntervalFormatStyle

Modifies the date interval format style to include the specified weekday style.

func year() -> Date.IntervalFormatStyle

Modifies the date interval format style to include the year.

### Comparing Date Interval Format Styles

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Date, Date) -> Bool

Returns true if the two `Date` values represent the same point in time.

### Supporting Types

typealias DateStyle

The type that defines date interval styles that vary in length or in their included components.

typealias Symbol

The type that supports customizing formatting templates using the date format style’s modifier functions, and constructing fixed-pattern date format strings.

typealias TimeStyle

The type that defines time styles that vary in length or in their included components.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- FormatStyle
- Hashable
- Sendable

## See Also

### Applying date and time styles

static var dateTime: Date.FormatStyle

A style for formatting a date and time.

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

static func relative(presentation: Date.RelativeFormatStyle.Presentation, unitsStyle: Date.RelativeFormatStyle.UnitsStyle) -> Self

Returns a style for formatting a date as relative to the current date.

struct RelativeFormatStyle

A format style that forms locale-aware string representations of a relative date or time.

static func components(style: Date.ComponentsFormatStyle.Style, fields: Set&lt;Date.ComponentsFormatStyle.Field>?) -> Self

Returns a style for formatting a date interval in terms of specific date components.

struct ComponentsFormatStyle

A style for formatting a date interval in terms of specific date components.

