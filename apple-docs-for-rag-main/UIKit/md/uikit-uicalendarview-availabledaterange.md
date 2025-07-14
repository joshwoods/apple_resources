

- UIKit
- UICalendarView
-  availableDateRange 

Instance Property

# availableDateRange

The range of dates that the calendar view displays.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var availableDateRange: DateInterval { get set }
```

## Discussion

Set `availableDateRange` to restrict the earliest or latest dates that the calendar view displays. The default date range starts with distantPast (Swift) or distantPast (Objective-C), and ends with distantFuture (Swift) or distantFuture (Objective-C).

## See Also

### Setting the visible date and range

var visibleDateComponents: DateComponents

The date components that represent the visible date in the calendar view.

func setVisibleDateComponents(DateComponents, animated: Bool)

Sets the date components that represent the date for the calendar view to make visible, with an option to animate the date change.

