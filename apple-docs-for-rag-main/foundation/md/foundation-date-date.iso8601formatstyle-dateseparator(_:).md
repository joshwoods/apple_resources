

- Foundation
- Date
- Date.ISO8601FormatStyle
-  dateSeparator(\_:) 

Instance Method

# dateSeparator(\_:)

Modifies the ISO 8601 date format style to use the specified date separator.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func dateSeparator(_ separator: Date.ISO8601FormatStyle.DateSeparator) -> Date.ISO8601FormatStyle
```

## Parameters 

`separator`  

Character used to separate the year, month, and day in a date.

## Return Value

An ISO 8601 date format style modified to include the specified date separator style.

## Discussion

Possible values of Date.ISO8601FormatStyle.DateSeparator are Date.ISO8601FormatStyle.DateSeparator.dash and Date.ISO8601FormatStyle.DateSeparator.omitted.

The following example shows a variety of Date.ISO8601FormatStyle.DateSeparator formats applied to an ISO 8601 date format.

```
let meetingDate = Date() // Jun 23, 2021 at 6:13 AM
meetingDate.formatted(.iso8601.dateSeparator(.omitted)) // 20210623T111325Z
meetingDate.formatted(.iso8601.dateSeparator(.dash)) // 2021-06-23T111325Z
meetingDate.formatted(.iso8601) // 20210623T111325Z
```

If no format is specified as a parameter, the Date.ISO8601FormatStyle.DateSeparator.omitted case is the default format.

For more information about ISO 8601 formatted dates, see the Date.ISO8601FormatStyle.

## See Also

### Modifying Dates in an ISO 8601 Format Style

func year() -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the year in the formatted output.

func month() -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the month in the formatted output.

func weekOfYear() -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the week of the year in the formatted output.

func day() -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the day in the formatted output.

