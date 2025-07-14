

- Foundation
- RelativeDateTimeFormatter
-  localizedString(from:) 

Instance Method

# localizedString(from:)

Formats a relative time represented by the specified date components.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func localizedString(from dateComponents: DateComponents) -> String
```

## Parameters 

`dateComponents`  

The date components to format.

## Return Value

A string that represents the formatted relative time from date components.

## Discussion

The formatter interprets a negative component value as a date in the past.

```
let components = DateComponents(day: -2)
let formatter = RelativeDateTimeFormatter()
print(formatter.localizedString(from: components))
// Outputs:  2 days ago
```

This method formats the value of the least granular unit in the NSDateComponents object, and doesn’t provide a compound format of the date component.

Important

This method only supports year, month, week of month, day, hour, minute, and second components. The formatter ignores all other date components.

## See Also

### Converting Dates to Formatted Strings

func localizedString(for: Date, relativeTo: Date) -> String

Formats the date interval from the reference date to the specified date using the formatter’s calendar.

func localizedString(fromTimeInterval: TimeInterval) -> String

Formats the specified time interval using the formatter’s calendar.

func string(for: Any?) -> String?

Creates a formatted string for a date relative to the current date and time.

