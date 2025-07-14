

- UIKit
- UITableView
-  hasActiveDrag 

Instance Property

# hasActiveDrag

A Boolean value that indicates whether the table view is currently tracking a drag session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var hasActiveDrag: Bool { get }
```

## See Also

### Managing drag interactions

var dragDelegate: (any UITableViewDragDelegate)?

The delegate object that manages the dragging of items from the table view.

protocol UITableViewDragDelegate

The interface for initiating drags from a table view.

var dragInteractionEnabled: Bool

A Boolean value that indicates whether the table view supports dragging content.

