

- UIKit
-  UICalendarSelection 

Class

# UICalendarSelection

A base object that tracks one or more dates a user selects from a calendar view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
class UICalendarSelection
```

## Overview

Don’t use this object directly in your calendar view to track date selection. Use the subclass UICalendarSelectionSingleDate to track a single date selection, or UICalendarSelectionMultiDate to track multiple date selections.

## Topics

### Updating selectable dates

func updateSelectableDates()

Informs the calendar view to update the view for selectable dates.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UICalendarSelectionMultiDate
- UICalendarSelectionSingleDate
- UICalendarSelectionWeekOfYear

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

class UICalendarSelectionSingleDate

An object that tracks a date the user selects from a calendar view.

class UICalendarSelectionMultiDate

An object that tracks multiple dates the user selects from a calendar view.

class UICalendarSelectionWeekOfYear

An object that tracks a specific week a person selects from a calendar view.

