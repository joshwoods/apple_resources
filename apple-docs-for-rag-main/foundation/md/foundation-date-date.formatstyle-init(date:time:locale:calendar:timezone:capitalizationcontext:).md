

- Foundation
- Date
- Date.FormatStyle
-  init(date:time:locale:calendar:timeZone:capitalizationContext:) 

Initializer

# init(date:time:locale:calendar:timeZone:capitalizationContext:)

Creates an instance using the provided date, time, locale, calendar, time zone, and capitalization context.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    date: Date.FormatStyle.DateStyle? = nil,
    time: Date.FormatStyle.TimeStyle? = nil,
    locale: Locale = .autoupdatingCurrent,
    calendar: Calendar = .autoupdatingCurrent,
    timeZone: TimeZone = .autoupdatingCurrent,
    capitalizationContext: FormatStyleCapitalizationContext = .unknown
)
```

## Parameters 

`date`  

The Date.FormatStyle.DateStyle used to create the string representation of the date.

`time`  

The Date.FormatStyle.TimeStyle used to create the string representation of the date.

`locale`  

The Locale used to create the string representation of the date.

`calendar`  

The Calendar used to create the string representation of the date.

`timeZone`  

The TimeZone used to create the string representation of the date.

`capitalizationContext`  

The FormatStyleCapitalizationContext used to create the string representation of the date.

## Discussion

Customize the date string by providing a date style, time style, locale, calendar, time zone, and capitalization scheme.

Date style values are complete, long, `abbreviated`, numeric, omitted, or `none`. Time style values are complete, standard, shortened, omitted, or `none`.

