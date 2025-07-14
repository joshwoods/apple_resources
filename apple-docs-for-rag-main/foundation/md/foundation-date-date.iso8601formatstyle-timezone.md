

- Foundation
- Date
- Date.ISO8601FormatStyle
-  timeZone 

Instance Property

# timeZone

The time zone used to create and parse date representations.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var timeZone: TimeZone { get set }
```

## Discussion

The default time zone is Greenwich Mean Time (GMT).

## See Also

### Modifying an ISO 8601 Format Style

var dateSeparator: Date.ISO8601FormatStyle.DateSeparator

The character used to separate the components of a date.

var dateTimeSeparator: Date.ISO8601FormatStyle.DateTimeSeparator

The character used to separate the date and time components of an ISO 8601 string representation of a date.

func dateTimeSeparator(Date.ISO8601FormatStyle.DateTimeSeparator) -> Date.ISO8601FormatStyle

Sets the character that specifies the date and time components.

