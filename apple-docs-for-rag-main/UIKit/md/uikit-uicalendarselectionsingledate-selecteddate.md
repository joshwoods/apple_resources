

- UIKit
- UICalendarSelectionSingleDate
-  selectedDate 

Instance Property

# selectedDate

A date component object that represents a selected date in a calendar view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var selectedDate: DateComponents? { get set }
```

## See Also

### Updating the selected date

func setSelected(DateComponents?, animated: Bool)

Updates the date component object that represents a selected date in a calendar view, with an option to animate the change.

