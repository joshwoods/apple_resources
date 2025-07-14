

- Foundation
- Date
- Date.ISO8601FormatStyle
-  timeZone(separator:) 

Instance Method

# timeZone(separator:)

Modifies the ISO 8601 date format style to include the time zone in the formatted output.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func timeZone(separator: Date.ISO8601FormatStyle.TimeZoneSeparator) -> Date.ISO8601FormatStyle
```

## Parameters 

`separator`  

Character used to separate the time and time zone in a date.

## Return Value

An ISO 8601 date format style modified to include the time zone.

## Discussion

The default Date.ISO8601FormatStyle doesn’t include the time zone.

For more information about formatting dates, see the Date.FormatStyle.

## See Also

### Modifying Times in an ISO 8601 Format Style

func time(includingFractionalSeconds: Bool) -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the time in the formatted output.

func timeSeparator(Date.ISO8601FormatStyle.TimeSeparator) -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to use the specified time separator.

func timeZoneSeparator(Date.ISO8601FormatStyle.TimeZoneSeparator) -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to use the specified time zone separator.

