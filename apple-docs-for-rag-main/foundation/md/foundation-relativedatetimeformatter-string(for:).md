

- Foundation
- RelativeDateTimeFormatter
-  string(for:) 

Instance Method

# string(for:)

Creates a formatted string for a date relative to the current date and time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func string(for obj: Any?) -> String?
```

## Parameters 

`obj`  

A date object to format.

## Return Value

A string that represents the date interval between a date and the current date and time, or `nil` if obj isn’t an instance of NSDate.

## Discussion

To determine the relative interval, the formatter uses date as the reference date.

## See Also

### Converting Dates to Formatted Strings

func localizedString(for: Date, relativeTo: Date) -> String

Formats the date interval from the reference date to the specified date using the formatter’s calendar.

func localizedString(from: DateComponents) -> String

Formats a relative time represented by the specified date components.

func localizedString(fromTimeInterval: TimeInterval) -> String

Formats the specified time interval using the formatter’s calendar.

