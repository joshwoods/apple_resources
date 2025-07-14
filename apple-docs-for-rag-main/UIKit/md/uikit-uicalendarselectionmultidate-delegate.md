

- UIKit
- UICalendarSelectionMultiDate
-  delegate 

Instance Property

# delegate

A delegate object that a calendar view asks for selectable dates and informs of changes to the selection of multiple dates.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UICalendarSelectionMultiDateDelegate)? { get }
```

## See Also

### Setting the selection delegate

protocol UICalendarSelectionMultiDateDelegate

A set of methods you implement to provide selectable dates and handle changes to the selection of multiple dates.

