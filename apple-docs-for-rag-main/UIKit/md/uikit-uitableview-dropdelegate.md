

- UIKit
- UITableView
-  dropDelegate 

Instance Property

# dropDelegate

The delegate object that manages the dropping of content into the table view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var dropDelegate: (any UITableViewDropDelegate)? { get set }
```

## Mentioned in 

Supporting drag and drop in table views

## See Also

### Managing drop interactions

protocol UITableViewDropDelegate

The interface for handling drops in a table view.

var hasActiveDrop: Bool

A Boolean value that indicates whether the table view is currently tracking a drop session.

