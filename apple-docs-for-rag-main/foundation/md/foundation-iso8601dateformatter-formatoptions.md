

- Foundation
- ISO8601DateFormatter
-  formatOptions 

Instance Property

# formatOptions

Options for generating and parsing ISO 8601 date representations. See ISO8601DateFormatter.Options for possible values.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var formatOptions: ISO8601DateFormatter.Options { get set }
```

## Discussion

The ISO 8601 specification allows for dates to be expressed in a variety of ways. You can configure the format used to parse and generate representations by specifying various combinations of format options.

| Format | Example | Options |
|----|----|----|
| Date with dash separators | `2016-06-13` | withFullDate, withDashSeparatorInDate |
| RFC 3339 Date and Time | `2016-06-13T16:00:00+00:00` | withInternetDateTime |
| Date and Time with space separator between date and time | `20160613 160000` | withFullDate, withFullTime, withSpaceBetweenDateAndTime |
| Week of Year | `2016-W24` | withYear, withWeekOfYear, withDashSeparatorInDate |
| Week of Year with Ordinal Weekday | `2016-W24-1` | withYear, withWeekOfYear, withDay, withDashSeparatorInDate |
| Ordinal Day of Year | `2016-165` | withYear, withDay, withDashSeparatorInDate |

Important

Resetting this property can incur a significant performance cost, as it may cause internal state to be regenerated.

## See Also

### Configuring the Formatter

var timeZone: TimeZone!

The time zone used to create and parse date representations. When unspecified, GMT is used.

