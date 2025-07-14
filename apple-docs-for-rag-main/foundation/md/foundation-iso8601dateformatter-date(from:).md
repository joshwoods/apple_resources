

- Foundation
- ISO8601DateFormatter
-  date(from:) 

Instance Method

# date(from:)

Creates and returns a date object from the specified ISO 8601 formatted string representation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func date(from string: String) -> Date?
```

## Parameters 

`string`  

The ISO 8601 formatted string representation of a date.

## Return Value

A date object, or `nil` if no valid date was found.

## See Also

### Converting ISO 8601 Dates

func string(from: Date) -> String

Creates and returns an ISO 8601 formatted string representation of the specified date.

class func string(from: Date, timeZone: TimeZone, formatOptions: ISO8601DateFormatter.Options) -> String

Creates a representation of the specified date with a given time zone and format options.

