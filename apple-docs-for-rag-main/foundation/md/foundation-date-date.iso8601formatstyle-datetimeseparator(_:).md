

- Foundation
- Date
- Date.ISO8601FormatStyle
-  dateTimeSeparator(\_:) 

Instance Method

# dateTimeSeparator(\_:)

Sets the character that specifies the date and time components.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func dateTimeSeparator(_ separator: Date.ISO8601FormatStyle.DateTimeSeparator) -> Date.ISO8601FormatStyle
```

## Parameters 

`separator`  

Possible values are `space` and `standard`.

## Return Value

An ISO 8601 date format style with the provided date and time component separator.

## Discussion

Possible values of Date.ISO8601FormatStyle.DateTimeSeparator are Date.ISO8601FormatStyle.DateTimeSeparator.space and Date.ISO8601FormatStyle.DateTimeSeparator.standard.

The following example shows a variety of Date.ISO8601FormatStyle.DateTimeSeparator formats applied to an ISO 8601 date format.

```
let meetingDate = Date() // Jun 23, 2021 at 10:21 AM
meetingDate.formatted(.iso8601.dateSeparator(.omitted)) // 20210623 152135Z
meetingDate.formatted(.iso8601.dateSeparator(.dash)) // 20210623T152135Z
meetingDate.formatted(.iso8601) // 20210623T152135Z
```

If no format is specified as a parameter, the Date.ISO8601FormatStyle.DateTimeSeparator.standard case is the default format.

For more information about ISO 8601 formatted dates, see the Date.ISO8601FormatStyle.

## See Also

### Modifying an ISO 8601 Format Style

var dateSeparator: Date.ISO8601FormatStyle.DateSeparator

The character used to separate the components of a date.

var dateTimeSeparator: Date.ISO8601FormatStyle.DateTimeSeparator

The character used to separate the date and time components of an ISO 8601 string representation of a date.

var timeZone: TimeZone

The time zone used to create and parse date representations.

