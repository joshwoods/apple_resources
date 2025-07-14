

- Foundation
- Date
- Date.ISO8601FormatStyle
-  timeSeparator(\_:) 

Instance Method

# timeSeparator(\_:)

Modifies the ISO 8601 date format style to use the specified time separator.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func timeSeparator(_ separator: Date.ISO8601FormatStyle.TimeSeparator) -> Date.ISO8601FormatStyle
```

## Parameters 

`separator`  

Character used to separate the hour and minute in a date.

## Return Value

An ISO 8601 date format style modified to include the specified time separator style.

## Discussion

Possible values of Date.ISO8601FormatStyle.TimeSeparator are Date.ISO8601FormatStyle.TimeSeparator.colon and Date.ISO8601FormatStyle.TimeSeparator.omitted.

This example shows a variety of ISO 8601 time separator formats applied to an ISO 8601 date format:

```
let meetingDate = Date() // Jun 23, 2021 at 1:41 PM
meetingDate.formatted(.iso8601.timeSeparator(.omitted)) // 20210623T184148Z
meetingDate.formatted(.iso8601.timeSeparator(.colon)) // 20210623T18:41:48Z
meetingDate.formatted(.iso8601) // 20210623T184148Z
```

If no format is specified as a parameter, the Date.ISO8601FormatStyle.DateSeparator.omitted case is the default format.

For more information about ISO 8601 formatted dates, see the Date.ISO8601FormatStyle.

## See Also

### Modifying Times in an ISO 8601 Format Style

func time(includingFractionalSeconds: Bool) -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the time in the formatted output.

func timeZone(separator: Date.ISO8601FormatStyle.TimeZoneSeparator) -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the time zone in the formatted output.

func timeZoneSeparator(Date.ISO8601FormatStyle.TimeZoneSeparator) -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to use the specified time zone separator.

