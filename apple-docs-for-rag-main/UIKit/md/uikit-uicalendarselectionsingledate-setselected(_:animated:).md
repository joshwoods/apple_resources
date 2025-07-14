

- UIKit
- UICalendarSelectionSingleDate
-  setSelected(\_:animated:) 

Instance Method

# setSelected(\_:animated:)

Updates the date component object that represents a selected date in a calendar view, with an option to animate the change.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func setSelected(
    _ selectedDate: DateComponents?,
    animated: Bool
)
```

## Parameters 

`selectedDate`  

A date component object that represents a date to select in a calendar view.

`animated`  

A Boolean value that indicates whether the calendar view should animate changing the selected date.

## See Also

### Updating the selected date

var selectedDate: DateComponents?

A date component object that represents a selected date in a calendar view.

