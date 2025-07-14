

- UIKit
- UICalendarSelectionMultiDateDelegate
-  multiDateSelection(\_:canSelectDate:) 

Instance Method

# multiDateSelection(\_:canSelectDate:)

Returns whether a user can select a date represented by date components in the calendar view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
optional func multiDateSelection(
    _ selection: UICalendarSelectionMultiDate,
    canSelectDate dateComponents: DateComponents
) -> Bool
```

## Parameters 

`selection`  

An object that tracks multiple dates that a user selects from a calendar view.

`dateComponents`  

Date components that represent a date to select.

## Return Value

A Boolean value that indicates whether the calendar view can select the date you provide.

## Discussion

The calendar view displays non-selectable dates as disabled.

## See Also

### Getting selectable dates

func multiDateSelection(UICalendarSelectionMultiDate, canDeselectDate: DateComponents) -> Bool

Returns whether a user can deselect a date represented by date components in the calendar view.

