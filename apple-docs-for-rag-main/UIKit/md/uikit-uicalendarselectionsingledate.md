

- UIKit
-  UICalendarSelectionSingleDate 

Class

# UICalendarSelectionSingleDate

An object that tracks a date the user selects from a calendar view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
class UICalendarSelectionSingleDate
```

## Topics

### Creating a single date selection

init(delegate: (any UICalendarSelectionSingleDateDelegate)?)

Creates an object that tracks a date a user selects from a calendar view, with an optional delegate to manage selectable dates and selection changes.

### Setting the selection delegate

var delegate: (any UICalendarSelectionSingleDateDelegate)?

A delegate object that a calendar view asks about selectable dates and informs of changes to the selection of a single date.

protocol UICalendarSelectionSingleDateDelegate

A set of methods you implement to provide selectable dates and handle changes to the selection of a single date.

### Updating the selected date

var selectedDate: DateComponents?

A date component object that represents a selected date in a calendar view.

func setSelected(DateComponents?, animated: Bool)

Updates the date component object that represents a selected date in a calendar view, with an option to animate the change.

## Relationships

### Inherits From

- UICalendarSelection

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Handling date selections

var selectionBehavior: UICalendarSelection?

The current date selection method of the calendar view.

class UICalendarSelectionMultiDate

An object that tracks multiple dates the user selects from a calendar view.

class UICalendarSelectionWeekOfYear

An object that tracks a specific week a person selects from a calendar view.

class UICalendarSelection

A base object that tracks one or more dates a user selects from a calendar view.

