

- UIKit
-  UICalendarSelectionSingleDateDelegate 

Protocol

# UICalendarSelectionSingleDateDelegate

A set of methods you implement to provide selectable dates and handle changes to the selection of a single date.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
protocol UICalendarSelectionSingleDateDelegate : NSObjectProtocol
```

## Topics

### Getting selectable dates

func dateSelection(UICalendarSelectionSingleDate, canSelectDate: DateComponents?) -> Bool

Returns whether a user can select a date represented by date components in the calendar view.

### Changing the selected date

func dateSelection(UICalendarSelectionSingleDate, didSelectDate: DateComponents?)

Informs the delegate that a user selected a date represented by date components.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting the selection delegate

var delegate: (any UICalendarSelectionSingleDateDelegate)?

A delegate object that a calendar view asks about selectable dates and informs of changes to the selection of a single date.

