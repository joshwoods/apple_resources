

- EventKit
- EKRecurrenceRule
-  init(recurrenceWith:interval:end:) 

Initializer

# init(recurrenceWith:interval:end:)

Initializes and returns a simple recurrence rule with a given frequency, interval, and end.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
init(
    recurrenceWith type: EKRecurrenceFrequency,
    interval: Int,
    end: EKRecurrenceEnd?
)
```

## Parameters 

`type`  

The frequency of the recurrence rule. Can be daily, weekly, monthly, or yearly.

`interval`  

The interval between instances of this recurrence. For example, a weekly recurrence rule with an interval of `2` occurs every other week. Must be greater than `0`.

`end`  

The end of the recurrence rule.

## Return Value

The initialized recurrence rule, or `nil` if invalid values are provided.

## Mentioned in 

Creating a recurring event

## See Also

### Related Documentation

Calendar and Reminders Programming Guide

### Creating a Basic Recurrence Rule

enum EKSpan

An object that indicates whether modifications should apply to a single event or all future events of a recurring event.

