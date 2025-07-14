

- Foundation
- Date
- Date.ISO8601FormatStyle
-  month() 

Instance Method

# month()

Modifies the ISO 8601 date format style to include the month in the formatted output.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func month() -> Date.ISO8601FormatStyle
```

## Return Value

An ISO 8601 date format style modified to include the month.

## Discussion

The following example shows an ISO 8601 format with, and without, a month.

```
let meetingDate = Date() // Jun 23, 2021 at 12:51 PM
meetingDate.formatted(.iso8601
    .year()
    .day()
) 
// 2021174

meetingDate.formatted(.iso8601
    .year()
    .month()
    .day()
) 
// 20210623
```

If `month()` isn’t included in the format but `day()` is, the format represents the day as the ordinal date.

The default Date.ISO8601FormatStyle includes the month.

For more information about formatting dates, see the Date.FormatStyle.

## See Also

### Modifying Dates in an ISO 8601 Format Style

func dateSeparator(Date.ISO8601FormatStyle.DateSeparator) -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to use the specified date separator.

func year() -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the year in the formatted output.

func weekOfYear() -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the week of the year in the formatted output.

func day() -> Date.ISO8601FormatStyle

Modifies the ISO 8601 date format style to include the day in the formatted output.

