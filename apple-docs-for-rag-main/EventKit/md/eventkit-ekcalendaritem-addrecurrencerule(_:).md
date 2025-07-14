

- EventKit
- EKCalendarItem
-  addRecurrenceRule(\_:) 

Instance Method

# addRecurrenceRule(\_:)

Adds a recurrence rule to the recurrence rule array.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func addRecurrenceRule(_ rule: EKRecurrenceRule)
```

## Parameters 

`rule`  

The rule to be added to recurrenceRules.

## Mentioned in 

Creating events and reminders

Creating a recurring event

## Discussion

The implementation only supports a single recurrence rule. Adding a recurrence rule replaces the single recurrence rule.

## See Also

### Setting Recurrence Rules

var hasRecurrenceRules: Bool

A Boolean value that indicates whether the calendar item has recurrence rules.

func removeRecurrenceRule(EKRecurrenceRule)

Removes a recurrence rule from the recurrence rule array.

var recurrenceRules: [EKRecurrenceRule]?

The recurrence rules for the calendar item.

