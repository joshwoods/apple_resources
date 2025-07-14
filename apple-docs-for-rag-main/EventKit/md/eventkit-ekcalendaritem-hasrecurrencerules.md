

- EventKit
- EKCalendarItem
-  hasRecurrenceRules 

Instance Property

# hasRecurrenceRules

A Boolean value that indicates whether the calendar item has recurrence rules.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var hasRecurrenceRules: Bool { get }
```

## Discussion

If true, the calendar item has recurrence rules; otherwise it does not.

### Special Considerations

The implementation only supports a single recurrence rule. Adding a recurrence rule replaces the single recurrence rule.

## See Also

### Setting Recurrence Rules

func addRecurrenceRule(EKRecurrenceRule)

Adds a recurrence rule to the recurrence rule array.

func removeRecurrenceRule(EKRecurrenceRule)

Removes a recurrence rule from the recurrence rule array.

var recurrenceRules: [EKRecurrenceRule]?

The recurrence rules for the calendar item.

