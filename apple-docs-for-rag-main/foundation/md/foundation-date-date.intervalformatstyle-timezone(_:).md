

- Foundation
- Date
- Date.IntervalFormatStyle
-  timeZone(\_:) 

Instance Method

# timeZone(\_:)

Modifies the date interval format style to use the specified time zone format.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func timeZone(_ format: Date.IntervalFormatStyle.Symbol.TimeZone = .genericName(.short)) -> Date.IntervalFormatStyle
```

## Parameters 

`format`  

The time zone format style for formatting a date interval.

## Return Value

A date interval format style with the provided time zone format.

## See Also

### Specifying Date Interval Format Styles

var calendar: Calendar

The calendar for formatting the date interval.

var locale: Locale

The locale for formatting the date and time interval components.

var timeZone: TimeZone

The time zone for formatting the date interval components.

