

- EventKit
- EKRecurrenceDayOfWeek
-  init(dayOfTheWeek:weekNumber:) 

Initializer

# init(dayOfTheWeek:weekNumber:)

Initializes and returns a day of the week with a given day and week number.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
init(
    dayOfTheWeek: EKWeekday,
    weekNumber: Int
)
```

## Parameters 

`dayOfTheWeek`  

The day of the week. Values range from `1` to `7`, with Sunday being `1`.

`weekNumber`  

The week number.

## Return Value

The initialized day of the week.

## See Also

### Creating a Day of the Week

enum EKWeekday

The day of the week.

convenience init(EKWeekday)

Creates and returns a day of the week with a given day.

convenience init(EKWeekday, weekNumber: Int)

Creates and returns an autoreleased day of the week with a given day and week number.

