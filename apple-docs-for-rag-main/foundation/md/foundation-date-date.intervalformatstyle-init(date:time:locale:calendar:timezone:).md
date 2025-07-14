

- Foundation
- Date
- Date.IntervalFormatStyle
-  init(date:time:locale:calendar:timeZone:) 

Initializer

# init(date:time:locale:calendar:timeZone:)

Creates an instance using the provided date, time, locale, calendar, time zone, and capitalization context.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    date: Date.IntervalFormatStyle.DateStyle? = nil,
    time: Date.IntervalFormatStyle.TimeStyle? = nil,
    locale: Locale = .autoupdatingCurrent,
    calendar: Calendar = .autoupdatingCurrent,
    timeZone: TimeZone = .autoupdatingCurrent
)
```

## Parameters 

`date`  

The Date.FormatStyle.DateStyle for creating the string representation of the date interval.

`time`  

The Date.FormatStyle.TimeStyle for creating the string representation of the date interval.

`locale`  

The Locale for creating the string representation of the date interval.

`calendar`  

The Calendar for creating the string representation of the date interval.

`timeZone`  

The TimeZone for creating the string representation of the date interval.

## Discussion

Customize the date interval string by providing a date style, time style, locale, calendar, time zone, and capitalization scheme.

Values for date style are complete, long, abbreviated, numeric, omitted, or `none`. Time style values are complete, standard, shortened, omitted, or `none`.

