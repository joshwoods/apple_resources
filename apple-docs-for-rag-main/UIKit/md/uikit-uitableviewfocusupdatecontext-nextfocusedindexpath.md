

- UIKit
- UITableViewFocusUpdateContext
-  nextFocusedIndexPath 

Instance Property

# nextFocusedIndexPath

Returns the index path of the cell containing the context’s next focused view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var nextFocusedIndexPath: IndexPath? { get }
```

## Discussion

This property returns the index path only when the nextFocusedView is located within a cell of the table view. Otherwise, it returns `nil`. This can happen if focus is moving out of the table view, because the nextFocusedView isn’t associated with an index path in this table view.

When focus is moving from one table view to another, each table view delegate is called with previouslyFocusedIndexPath and nextFocusedIndexPath configured for its specific table view.

## See Also

### Locating focusable items in a table view

var previouslyFocusedIndexPath: IndexPath?

Returns the index path of the cell containing the context’s previously focused view.

