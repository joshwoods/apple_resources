

- UIKit
- UICalendarSelectionMultiDate
-  selectedDates 

Instance Property

# selectedDates

An array of date component objects that represent selected dates in a calendar view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var selectedDates: [DateComponents] { get set }
```

## See Also

### Updating the selected dates

func setSelectedDates([DateComponents], animated: Bool)

Updates the array of date component objects that represent selected dates in a calendar view, with an option to animate the change.

