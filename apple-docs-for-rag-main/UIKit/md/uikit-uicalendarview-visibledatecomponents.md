

- UIKit
- UICalendarView
-  visibleDateComponents 

Instance Property

# visibleDateComponents

The date components that represent the visible date in the calendar view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var visibleDateComponents: DateComponents { get set }
```

## Discussion

If `visibleDateComponents.calendar` is `nil` or isn’t equal to calendar, the calendar view uses calendar, which may result in an invalid date from the date components.

## See Also

### Setting the visible date and range

func setVisibleDateComponents(DateComponents, animated: Bool)

Sets the date components that represent the date for the calendar view to make visible, with an option to animate the date change.

var availableDateRange: DateInterval

The range of dates that the calendar view displays.

