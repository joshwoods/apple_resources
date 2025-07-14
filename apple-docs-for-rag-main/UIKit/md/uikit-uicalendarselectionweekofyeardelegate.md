

- UIKit
-  UICalendarSelectionWeekOfYearDelegate 

Protocol

# UICalendarSelectionWeekOfYearDelegate

A set of methods you implement to provide selectable weeks and handle changes to the week selection in a calendar view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@MainActor
protocol UICalendarSelectionWeekOfYearDelegate : NSObjectProtocol
```

## Topics

### Handling week-of-year selections

func week(ofYearSelection: UICalendarSelectionWeekOfYear, canSelectWeekOfYear: DateComponents?) -> Bool

Notifies the delegate after a person selects a week in the calendar view.

func week(ofYearSelection: UICalendarSelectionWeekOfYear, didSelectWeekOfYear: DateComponents?)

Determines if a week is available for selection.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Setting the selection delegate

var delegate: (any UICalendarSelectionWeekOfYearDelegate)?

A delegate object that a calendar view asks about selectable weeks and informs of changes to the week selection.

