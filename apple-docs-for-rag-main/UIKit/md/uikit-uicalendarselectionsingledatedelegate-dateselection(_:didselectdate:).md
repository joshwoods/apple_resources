

- UIKit
- UICalendarSelectionSingleDateDelegate
-  dateSelection(\_:didSelectDate:) 

Instance Method

# dateSelection(\_:didSelectDate:)

Informs the delegate that a user selected a date represented by date components.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func dateSelection(
    _ selection: UICalendarSelectionSingleDate,
    didSelectDate dateComponents: DateComponents?
)
```

**Required**

## Parameters 

`selection`  

An object that tracks a date that a user selects from a calendar view.

`dateComponents`  

Date components that represent a date the user selected, or `nil` if the user deselected a date.

