

- Foundation
- Date
-  ISO8601Format(\_:) 

Instance Method

# ISO8601Format(\_:)

Generates a locale-aware string representation of a date using the ISO 8601 date format.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func ISO8601Format(_ style: Date.ISO8601FormatStyle = .init()) -> String
```

## Parameters 

`style`  

A customized Date.ISO8601FormatStyle to apply. By default, the method applies an unmodified ISO 8601 format style.

## Return Value

A string, formatted according to the specified style.

## Discussion

Calling this method is equivalent to passing a Date.ISO8601FormatStyle to a date’s formatted() method.

## See Also

### Formatting a Date

func formatted() -> String

Generates a locale-aware string representation of a date using the default date format style.

func formatted(date: Date.FormatStyle.DateStyle, time: Date.FormatStyle.TimeStyle) -> String

Generates a locale-aware string representation of a date using specified date and time format styles.

func formatted&lt;F>(F) -> F.FormatOutput

Generates a locale-aware string representation of a date using the specified date format style.

struct FormatStyle

A structure that creates a locale-appropriate string representation of a date instance and converts strings of dates and times into date instances.

struct RelativeFormatStyle

A format style that forms locale-aware string representations of a relative date or time.

struct IntervalFormatStyle

A format style that creates string representations of date intervals.

struct ISO8601FormatStyle

A type that converts between dates and their ISO-8601 string representations.

