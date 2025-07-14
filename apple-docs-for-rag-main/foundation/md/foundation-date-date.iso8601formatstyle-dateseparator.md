

- Foundation
- Date
- Date.ISO8601FormatStyle
-  dateSeparator 

Instance Property

# dateSeparator

The character used to separate the components of a date.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var dateSeparator: Date.ISO8601FormatStyle.DateSeparator { get }
```

## See Also

### Modifying an ISO 8601 Format Style

var dateTimeSeparator: Date.ISO8601FormatStyle.DateTimeSeparator

The character used to separate the date and time components of an ISO 8601 string representation of a date.

var timeZone: TimeZone

The time zone used to create and parse date representations.

func dateTimeSeparator(Date.ISO8601FormatStyle.DateTimeSeparator) -> Date.ISO8601FormatStyle

Sets the character that specifies the date and time components.

