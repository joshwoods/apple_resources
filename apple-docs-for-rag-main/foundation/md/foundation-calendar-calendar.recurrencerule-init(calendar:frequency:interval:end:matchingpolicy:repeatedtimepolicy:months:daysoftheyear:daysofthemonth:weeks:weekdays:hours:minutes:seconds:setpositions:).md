

- Foundation
- Calendar
- Calendar.RecurrenceRule
-  init(calendar:frequency:interval:end:matchingPolicy:repeatedTimePolicy:months:daysOfTheYear:daysOfTheMonth:weeks:weekdays:hours:minutes:seconds:setPositions:) 

Initializer

# init(calendar:frequency:interval:end:matchingPolicy:repeatedTimePolicy:months:daysOfTheYear:daysOfTheMonth:weeks:weekdays:hours:minutes:seconds:setPositions:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    calendar: Calendar,
    frequency: Calendar.RecurrenceRule.Frequency,
    interval: Int = 1,
    end: Calendar.RecurrenceRule.End = .never,
    matchingPolicy: Calendar.MatchingPolicy = .nextTimePreservingSmallerComponents,
    repeatedTimePolicy: Calendar.RepeatedTimePolicy = .first,
    months: [Calendar.RecurrenceRule.Month] = [],
    daysOfTheYear: [Int] = [],
    daysOfTheMonth: [Int] = [],
    weeks: [Int] = [],
    weekdays: [Calendar.RecurrenceRule.Weekday] = [],
    hours: [Int] = [],
    minutes: [Int] = [],
    seconds: [Int] = [],
    setPositions: [Int] = []
)
```

