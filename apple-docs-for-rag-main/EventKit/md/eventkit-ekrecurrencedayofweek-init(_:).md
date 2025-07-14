

- EventKit
- EKRecurrenceDayOfWeek
-  init(\_:) 

Initializer

# init(\_:)

Creates and returns a day of the week with a given day.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
convenience init(_ dayOfTheWeek: EKWeekday)
```

## Parameters 

`dayOfTheWeek`  

The day of the week. Values range from `1` to `7`, with Sunday being `1`.

## Return Value

The new day of the week.

## Discussion

The week number of the returned day of the week is `0`.

## See Also

### Creating a Day of the Week

enum EKWeekday

The day of the week.

convenience init(EKWeekday, weekNumber: Int)

Creates and returns an autoreleased day of the week with a given day and week number.

init(dayOfTheWeek: EKWeekday, weekNumber: Int)

Initializes and returns a day of the week with a given day and week number.

