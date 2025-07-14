

- Foundation
- Date
-  formatted(date:time:) 

Instance Method

# formatted(date:time:)

Generates a locale-aware string representation of a date using specified date and time format styles.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func formatted(
    date: Date.FormatStyle.DateStyle,
    time: Date.FormatStyle.TimeStyle
) -> String
```

## Parameters 

`date`  

The date format style to apply to the date.

`time`  

The time format style to apply to the date.

## Return Value

A string, formatted according to the specified date and time styles.

## Discussion

When displaying a date to a user, use the convenient formatted(date:time:) instance method to customize the string representation of the date. Set the date and time styles of the date format style separately, according to your particular needs.

For example, to create a string with a full date and no time representation, set the Date.FormatStyle.DateStyle to complete and the Date.FormatStyle.TimeStyle to omitted. Conversely, to create a string representing only the time, set the date style to omitted and the time style to complete.

```
let birthday = Date()

birthday.formatted(date: .complete, time: .omitted) // Sunday, January 17, 2021
birthday.formatted(date: .omitted, time: .complete) // 4:03:12 PM CST
```

You can create string representations of a Date instance with several levels of brevity using a variety of preset date and time styles. This example shows date styles of long, abbreviated, and numeric, and time styles of shortened, standard, and complete.

```
let birthday = Date()

birthday.formatted(date: .long, time: .shortened) // January 17, 2021, 4:03 PM
birthday.formatted(date: .abbreviated, time: .standard) // Jan 17, 2021, 4:03:12 PM
birthday.formatted(date: .numeric, time: .complete) // 1/17/2021, 4:03:12 PM CST

birthday.formatted() // Jan 17, 2021, 4:03 PM
```

The default date style is abbreviated and the default time style is shortened.

For the default date formatting, use the formatted() method. To customize the formatted measurement string, use the formatted(_:) method and include a `Date.FormatStyle`.

For more information about formatting dates, see the Date.FormatStyle.

## See Also

### Formatting a Date

func formatted() -> String

Generates a locale-aware string representation of a date using the default date format style.

func formatted&lt;F>(F) -> F.FormatOutput

Generates a locale-aware string representation of a date using the specified date format style.

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

