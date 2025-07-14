

- EventKit
- EKCalendarItem
-  removeRecurrenceRule(\_:) 

Instance Method

# removeRecurrenceRule(\_:)

Removes a recurrence rule from the recurrence rule array.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
func removeRecurrenceRule(_ rule: EKRecurrenceRule)
```

## Parameters 

`rule`  

The rule to be removed from recurrenceRules.

## Discussion

The implementation only supports a single recurrence rule.

## See Also

### Setting Recurrence Rules

var hasRecurrenceRules: Bool

A Boolean value that indicates whether the calendar item has recurrence rules.

func addRecurrenceRule(EKRecurrenceRule)

Adds a recurrence rule to the recurrence rule array.

var recurrenceRules: [EKRecurrenceRule]?

The recurrence rules for the calendar item.

