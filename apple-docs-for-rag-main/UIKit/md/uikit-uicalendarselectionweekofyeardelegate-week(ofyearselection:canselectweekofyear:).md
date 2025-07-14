

- UIKit
- UICalendarSelectionWeekOfYearDelegate
-  week(ofYearSelection:canSelectWeekOfYear:) 

Instance Method

# week(ofYearSelection:canSelectWeekOfYear:)

Notifies the delegate after a person selects a week in the calendar view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@MainActor
optional func week(
    ofYearSelection selection: UICalendarSelectionWeekOfYear,
    canSelectWeekOfYear weekOfYearComponents: DateComponents?
) -> Bool
```

## See Also

### Handling week-of-year selections

func week(ofYearSelection: UICalendarSelectionWeekOfYear, didSelectWeekOfYear: DateComponents?)

Determines if a week is available for selection.

**Required**

