

- Foundation
-  ISO8601DateFormatter 

Class

# ISO8601DateFormatter

A formatter that converts between dates and their ISO 8601 string representations.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class ISO8601DateFormatter
```

## Overview

The ISO8601DateFormatter class generates and parses string representations of dates following the ISO 8601 standard. Use this class to create ISO 8601 representations of dates and create dates from text strings in ISO 8601 format.

Tip

In Swift, you can use Date.ISO8601FormatStyle rather than ISO8601DateFormatter. The FormatStyle API offers a declarative idiom for customizing the formatting of various types. Also, Foundation caches identical FormatStyle instances, so you don’t need to pass them around your app, or risk wasting memory with duplicate formatters.

## Topics

### Configuring the Formatter

var formatOptions: ISO8601DateFormatter.Options

Options for generating and parsing ISO 8601 date representations. See ISO8601DateFormatter.Options for possible values.

var timeZone: TimeZone!

The time zone used to create and parse date representations. When unspecified, GMT is used.

### Creating ISO 8601 Date Formatters

init()

Initializes an ISO 8601 date formatter with default format, time zone, and options.

### Converting ISO 8601 Dates

func string(from: Date) -> String

Creates and returns an ISO 8601 formatted string representation of the specified date.

func date(from: String) -> Date?

Creates and returns a date object from the specified ISO 8601 formatted string representation.

class func string(from: Date, timeZone: TimeZone, formatOptions: ISO8601DateFormatter.Options) -> String

Creates a representation of the specified date with a given time zone and format options.

### Constants

struct Options

Options used to generate and parse ISO 8601 date representations.

## Relationships

### Inherits From

- Formatter

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Dates and times

class DateFormatter

A formatter that converts between dates and their textual representations.

class DateComponentsFormatter

A formatter that creates string representations of quantities of time.

class RelativeDateTimeFormatter

A formatter that creates locale-aware string representations of a relative date or time.

class DateIntervalFormatter

A formatter that creates string representations of time intervals.

