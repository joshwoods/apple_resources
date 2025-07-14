

- Foundation
- RelativeDateTimeFormatter
-  localizedString(fromTimeInterval:) 

Instance Method

# localizedString(fromTimeInterval:)

Formats the specified time interval using the formatter’s calendar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func localizedString(fromTimeInterval timeInterval: TimeInterval) -> String
```

## Parameters 

`timeInterval`  

The time interval to format.

## Return Value

A string that represents the formatted time interval.

## Discussion

The formatter interprets a negative time interval as a date in the past.

```
let formatter = RelativeDateTimeFormatter()
print(formatter.localizedString(fromTimeInterval: -120))
// Outputs:  2 minutes ago
```

## See Also

### Converting Dates to Formatted Strings

func localizedString(for: Date, relativeTo: Date) -> String

Formats the date interval from the reference date to the specified date using the formatter’s calendar.

func localizedString(from: DateComponents) -> String

Formats a relative time represented by the specified date components.

func string(for: Any?) -> String?

Creates a formatted string for a date relative to the current date and time.

