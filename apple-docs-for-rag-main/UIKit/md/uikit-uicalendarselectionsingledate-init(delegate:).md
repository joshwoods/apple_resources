

- UIKit
- UICalendarSelectionSingleDate
-  init(delegate:) 

Initializer

# init(delegate:)

Creates an object that tracks a date a user selects from a calendar view, with an optional delegate to manage selectable dates and selection changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
init(delegate: (any UICalendarSelectionSingleDateDelegate)?)
```

## Parameters 

`delegate`  

A delegate object that a calendar view asks about selectable dates, and informs of changes to the selection of a single date.

