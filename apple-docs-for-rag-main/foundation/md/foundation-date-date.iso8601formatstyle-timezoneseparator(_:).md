

- Foundation
- Date
- Date.ISO8601FormatStyle
-  timeZoneSeparator(\_:) 

Instance Method

# timeZoneSeparator(\_:)

Modifies the ISO 8601 date format style to use the specified time zone separator.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func timeZoneSeparator(_ separator: Date.ISO8601FormatStyle.TimeZoneSeparator) -> Date.ISO8601FormatStyle
```

## Parameters 

`separator`  

Character used to separate the time and time zone in a date.

## Return Value

An ISO 8601 date format style modified to include the specified time zone separator style.

## Discussion

Possible values of Date.ISO8601FormatStyle.TimeZoneSeparator are Date.ISO8601FormatStyle.TimeZoneSeparator.colon and Date.ISO8601FormatStyle.TimeZoneSeparator.omitted.

For more information about ISO 8601 formatted dates, see the Date.ISO8601FormatStyle.

## See Also

### Modifying Times in an ISO 8601 Format Style

func time(includingFractionalSeconds: Bool) -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the time in the formatted output.

func timeSeparator(Date.ISO8601FormatStyle.TimeSeparator) -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to use the specified time separator.

func timeZone(separator: Date.ISO8601FormatStyle.TimeZoneSeparator) -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the time zone in the formatted output.

