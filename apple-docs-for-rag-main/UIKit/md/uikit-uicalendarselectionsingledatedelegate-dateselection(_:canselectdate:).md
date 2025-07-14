

- UIKit
- UICalendarSelectionSingleDateDelegate
-  dateSelection(\_:canSelectDate:) 

Instance Method

# dateSelection(\_:canSelectDate:)

Returns whether a user can select a date represented by date components in the calendar view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
optional func dateSelection(
    _ selection: UICalendarSelectionSingleDate,
    canSelectDate dateComponents: DateComponents?
) -> Bool
```

## Parameters 

`selection`  

An object that tracks a date that a user selects from a calendar view.

`dateComponents`  

Date components that represent a date to select.

## Return Value

A Boolean value that indicates whether the calendar view can select the date you provide.

## Discussion

The calendar view displays nonselectable dates as disabled.

