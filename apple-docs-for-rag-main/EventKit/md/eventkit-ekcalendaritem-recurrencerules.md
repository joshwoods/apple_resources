

- EventKit
- EKCalendarItem
-  recurrenceRules 

Instance Property

# recurrenceRules

The recurrence rules for the calendar item.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var recurrenceRules: [EKRecurrenceRule]? { get set }
```

## Discussion

The implementation only supports a single recurrence rule.

## See Also

### Setting Recurrence Rules

var hasRecurrenceRules: Bool

A Boolean value that indicates whether the calendar item has recurrence rules.

func addRecurrenceRule(EKRecurrenceRule)

Adds a recurrence rule to the recurrence rule array.

func removeRecurrenceRule(EKRecurrenceRule)

Removes a recurrence rule from the recurrence rule array.

