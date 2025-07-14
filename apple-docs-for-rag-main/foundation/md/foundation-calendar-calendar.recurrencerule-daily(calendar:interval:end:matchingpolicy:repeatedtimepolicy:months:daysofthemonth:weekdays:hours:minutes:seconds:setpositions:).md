

- Foundation
- Calendar
- Calendar.RecurrenceRule
-  daily(calendar:interval:end:matchingPolicy:repeatedTimePolicy:months:daysOfTheMonth:weekdays:hours:minutes:seconds:setPositions:) 

Type Method

# daily(calendar:interval:end:matchingPolicy:repeatedTimePolicy:months:daysOfTheMonth:weekdays:hours:minutes:seconds:setPositions:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
static func daily(
    calendar: Calendar,
    interval: Int = 1,
    end: Calendar.RecurrenceRule.End = .never,
    matchingPolicy: Calendar.MatchingPolicy = .nextTimePreservingSmallerComponents,
    repeatedTimePolicy: Calendar.RepeatedTimePolicy = .first,
    months: [Calendar.RecurrenceRule.Month] = [],
    daysOfTheMonth: [Int] = [],
    weekdays: [Calendar.RecurrenceRule.Weekday] = [],
    hours: [Int] = [],
    minutes: [Int] = [],
    seconds: [Int] = [],
    setPositions: [Int] = []
) -> Calendar.RecurrenceRule
```

