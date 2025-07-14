

- UIKit
- UICalendarView
-  setVisibleDateComponents(\_:animated:) 

Instance Method

# setVisibleDateComponents(\_:animated:)

Sets the date components that represent the date for the calendar view to make visible, with an option to animate the date change.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func setVisibleDateComponents(
    _ dateComponents: DateComponents,
    animated: Bool
)
```

## Parameters 

`dateComponents`  

Date components that represent the date for the calendar view to display.

`animated`  

A Boolean value that indicates whether the calendar view animates the date change.

## Discussion

The date that `dateComponents` represents must be within the dates that availableDateRange represents.

If `dateComponents.calendar` is `nil` or isn’t equal to calendar, the calendar view uses calendar, which may result in an invalid date from the date components.

## See Also

### Setting the visible date and range

var visibleDateComponents: DateComponents

The date components that represent the visible date in the calendar view.

var availableDateRange: DateInterval

The range of dates that the calendar view displays.

