

- UIKit
- UICalendarSelectionWeekOfYear
-  setSelected(\_:animated:) 

Instance Method

# setSelected(\_:animated:)

Updates the date component object that represents a selected week in a calendar view, with an option to animate the change.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@MainActor
func setSelected(
    _ selectedWeekOfYear: DateComponents?,
    animated: Bool
)
```

## See Also

### Updating the selected week

var selectedWeekOfYear: DateComponents?

The current week-of-year selection in the calendar view.

