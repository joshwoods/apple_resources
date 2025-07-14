

- Foundation
- RelativeDateTimeFormatter
-  localizedString(for:relativeTo:) 

Instance Method

# localizedString(for:relativeTo:)

Formats the date interval from the reference date to the specified date using the formatter’s calendar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func localizedString(
    for date: Date,
    relativeTo referenceDate: Date
) -> String
```

## Parameters 

`date`  

The end date of the interval to format.

`referenceDate`  

The start date of the interval to format.

## Return Value

A string that represents the date interval between two dates.

## Discussion

```
let tenMinutesAgo = Date(timeIntervalSinceNow: -600)
let twoMintuesAhead = Date(timeIntervalSinceNow: 120)
let formatter = RelativeDateTimeFormatter()
print(formatter.localizedString(for: tenMinutesAgo, relativeTo: twoMintuesAhead))
// Outputs: 12 minutes ago
```

## See Also

### Converting Dates to Formatted Strings

func localizedString(from: DateComponents) -> String

Formats a relative time represented by the specified date components.

func localizedString(fromTimeInterval: TimeInterval) -> String

Formats the specified time interval using the formatter’s calendar.

func string(for: Any?) -> String?

Creates a formatted string for a date relative to the current date and time.

