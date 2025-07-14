

- UIKit
- UICalendarSelectionWeekOfYear
-  delegate 

Instance Property

# delegate

A delegate object that a calendar view asks about selectable weeks and informs of changes to the week selection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
@MainActor
weak var delegate: (any UICalendarSelectionWeekOfYearDelegate)? { get }
```

## See Also

### Setting the selection delegate

protocol UICalendarSelectionWeekOfYearDelegate

A set of methods you implement to provide selectable weeks and handle changes to the week selection in a calendar view.

