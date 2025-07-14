

- UIKit
- UITableView
-  dragDelegate 

Instance Property

# dragDelegate

The delegate object that manages the dragging of items from the table view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var dragDelegate: (any UITableViewDragDelegate)? { get set }
```

## Mentioned in 

Supporting drag and drop in table views

## See Also

### Managing drag interactions

protocol UITableViewDragDelegate

The interface for initiating drags from a table view.

var hasActiveDrag: Bool

A Boolean value that indicates whether the table view is currently tracking a drag session.

var dragInteractionEnabled: Bool

A Boolean value that indicates whether the table view supports dragging content.

