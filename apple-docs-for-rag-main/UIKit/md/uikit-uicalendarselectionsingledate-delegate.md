

- UIKit
- UICalendarSelectionSingleDate
-  delegate 

Instance Property

# delegate

A delegate object that a calendar view asks about selectable dates and informs of changes to the selection of a single date.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UICalendarSelectionSingleDateDelegate)? { get }
```

## See Also

### Setting the selection delegate

protocol UICalendarSelectionSingleDateDelegate

A set of methods you implement to provide selectable dates and handle changes to the selection of a single date.

