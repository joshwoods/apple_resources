

- UIKit
-  UICalendarSelectionMultiDateDelegate 

Protocol

# UICalendarSelectionMultiDateDelegate

A set of methods you implement to provide selectable dates and handle changes to the selection of multiple dates.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
protocol UICalendarSelectionMultiDateDelegate : NSObjectProtocol
```

## Topics

### Getting selectable dates

func multiDateSelection(UICalendarSelectionMultiDate, canSelectDate: DateComponents) -> Bool

Returns whether a user can select a date represented by date components in the calendar view.

func multiDateSelection(UICalendarSelectionMultiDate, canDeselectDate: DateComponents) -> Bool

Returns whether a user can deselect a date represented by date components in the calendar view.

### Changing selected dates

func multiDateSelection(UICalendarSelectionMultiDate, didSelectDate: DateComponents)

Informs the delegate that a user selected a date represented by date components.

**Required**

func multiDateSelection(UICalendarSelectionMultiDate, didDeselectDate: DateComponents)

Informs the delegate that a user deselected a date represented by date components.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting the selection delegate

var delegate: (any UICalendarSelectionMultiDateDelegate)?

A delegate object that a calendar view asks for selectable dates and informs of changes to the selection of multiple dates.

