

- UIKit
- UICalendarSelectionMultiDate
-  init(delegate:) 

Initializer

# init(delegate:)

Creates an object that tracks multiple dates a user selects from a calendar view, with an optional delegate to manage selectable dates and selection changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
init(delegate: (any UICalendarSelectionMultiDateDelegate)?)
```

## Parameters 

`delegate`  

A delegate object that a calendar view asks for selectable dates, and informs of changes to the selection of multiple dates.

