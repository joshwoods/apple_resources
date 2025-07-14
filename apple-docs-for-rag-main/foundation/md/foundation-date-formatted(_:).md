

- Foundation
- Date
-  formatted(\_:) 

Instance Method

# formatted(\_:)

Generates a locale-aware string representation of a date using the specified date format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func formatted(_ format: F) -> F.FormatOutput where F : FormatStyle, F.FormatInput == Date
```

## Parameters 

`format`  

The date format style to apply to the date.

## Return Value

A string, formatted according to the specified style.

## Discussion

For full customization of the string representation of a date, use the formatted(_:) instance method of Date and provide a Date.FormatStyle object.

You can achieve any customization of date and time representation your app requires by appying a series of convenience modifiers to your format style. This example applies a series of modifiers to the format style to precisely define the formatting of the year, month, day, hour, minute, and timezone components of the resulting string.

```
// Call the .formatted method on an instance of Date passing in an instance of Date.FormatStyle.

let birthday = Date()

birthday.formatted(
    Date.FormatStyle()
        .year(.defaultDigits)
        .month(.abbreviated)
        .day(.twoDigits)
        .hour(.defaultDigits(amPM: .abbreviated))
        .minute(.twoDigits)
        .timeZone(.identifier(.long))
        .era(.wide)
        .dayOfYear(.defaultDigits)
        .weekday(.abbreviated)
        .week(.defaultDigits)
) 
// Sun, Jan 17, 2021 Anno Domini (week: 4), 11:18 AM America/Chicago
```

For the default date formatting, use the formatted() method. For basic customization of the formatted date string, use the formatted(date:time:) and include a date and time style.

For more information about formatting dates, see Date.FormatStyle.

## See Also

### Formatting a Date

func formatted() -> String

Generates a locale-aware string representation of a date using the default date format style.

func formatted(date: Date.FormatStyle.DateStyle, time: Date.FormatStyle.TimeStyle) -> String

Generates a locale-aware string representation of a date using specified date and time format styles.

struct FormatStyle

A structure that creates a locale-appropriate string representation of a date instance and converts strings of dates and times into date instances.

struct RelativeFormatStyle

A format style that forms locale-aware string representations of a relative date or time.

struct IntervalFormatStyle

A format style that creates string representations of date intervals.

func ISO8601Format(Date.ISO8601FormatStyle) -> String

Generates a locale-aware string representation of a date using the ISO 8601 date format.

struct ISO8601FormatStyle

A type that converts between dates and their ISO-8601 string representations.

