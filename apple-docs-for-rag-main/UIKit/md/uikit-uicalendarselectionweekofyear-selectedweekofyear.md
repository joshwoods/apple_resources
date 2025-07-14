

- UIKit
- UICalendarSelectionWeekOfYear
-  selectedWeekOfYear 

Instance Property

# selectedWeekOfYear

The current week-of-year selection in the calendar view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@MainActor
var selectedWeekOfYear: DateComponents? { get set }
```

## Discussion

The components need to include `[.yearForWeekOfYear, .weekOfYear]`.

## See Also

### Updating the selected week

func setSelected(DateComponents?, animated: Bool)

Updates the date component object that represents a selected week in a calendar view, with an option to animate the change.

