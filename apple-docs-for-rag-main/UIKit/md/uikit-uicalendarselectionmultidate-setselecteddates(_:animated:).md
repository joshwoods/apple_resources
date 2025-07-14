

- UIKit
- UICalendarSelectionMultiDate
-  setSelectedDates(\_:animated:) 

Instance Method

# setSelectedDates(\_:animated:)

Updates the array of date component objects that represent selected dates in a calendar view, with an option to animate the change.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func setSelectedDates(
    _ selectedDates: [DateComponents],
    animated: Bool
)
```

## Parameters 

`selectedDates`  

An array of date component objects that represent dates to select in a calendar view.

`animated`  

A Boolean value that indicates whether the calendar view should animate changing the selected dates.

## See Also

### Updating the selected dates

var selectedDates: [DateComponents]

An array of date component objects that represent selected dates in a calendar view.

