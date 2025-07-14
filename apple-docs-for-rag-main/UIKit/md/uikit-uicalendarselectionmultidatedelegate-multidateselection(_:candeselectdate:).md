

- UIKit
- UICalendarSelectionMultiDateDelegate
-  multiDateSelection(\_:canDeselectDate:) 

Instance Method

# multiDateSelection(\_:canDeselectDate:)

Returns whether a user can deselect a date represented by date components in the calendar view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
optional func multiDateSelection(
    _ selection: UICalendarSelectionMultiDate,
    canDeselectDate dateComponents: DateComponents
) -> Bool
```

## Parameters 

`selection`  

An object that tracks one or more dates that a user selects from a calendar view.

`dateComponents`  

Date components that represent a date to deselect.

## Return Value

A Boolean value that indicates whether the calendar view can deselect the date you provide.

## See Also

### Getting selectable dates

func multiDateSelection(UICalendarSelectionMultiDate, canSelectDate: DateComponents) -> Bool

Returns whether a user can select a date represented by date components in the calendar view.

