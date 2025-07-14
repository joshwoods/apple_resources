

- UIKit
- UICalendarSelectionWeekOfYearDelegate
-  week(ofYearSelection:didSelectWeekOfYear:) 

Instance Method

# week(ofYearSelection:didSelectWeekOfYear:)

Determines if a week is available for selection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@MainActor
func week(
    ofYearSelection selection: UICalendarSelectionWeekOfYear,
    didSelectWeekOfYear weekOfYearComponents: DateComponents?
)
```

**Required**

## See Also

### Handling week-of-year selections

func week(ofYearSelection: UICalendarSelectionWeekOfYear, canSelectWeekOfYear: DateComponents?) -> Bool

Notifies the delegate after a person selects a week in the calendar view.

