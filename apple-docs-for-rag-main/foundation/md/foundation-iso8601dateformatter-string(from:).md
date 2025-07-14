

- Foundation
- ISO8601DateFormatter
-  string(from:) 

Instance Method

# string(from:)

Creates and returns an ISO 8601 formatted string representation of the specified date.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func string(from date: Date) -> String
```

## Parameters 

`date`  

The date to be represented.

## Return Value

A user-readable string representing the date.

## See Also

### Converting ISO 8601 Dates

func date(from: String) -> Date?

Creates and returns a date object from the specified ISO 8601 formatted string representation.

class func string(from: Date, timeZone: TimeZone, formatOptions: ISO8601DateFormatter.Options) -> String

Creates a representation of the specified date with a given time zone and format options.

