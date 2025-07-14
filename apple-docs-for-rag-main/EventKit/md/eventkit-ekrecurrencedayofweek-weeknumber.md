

- EventKit
- EKRecurrenceDayOfWeek
-  weekNumber 

Instance Property

# weekNumber

The week number of the day of the week.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var weekNumber: Int { get }
```

## Discussion

Values range from `–53` to `53`. A negative value indicates a value from the end of the range. `0` indicates the week number is irrelevant.

## See Also

### Accessing Properties of a Day of the Week

var dayOfTheWeek: EKWeekday

The day of the week.

