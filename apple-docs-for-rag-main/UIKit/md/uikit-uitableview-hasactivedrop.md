

- UIKit
- UITableView
-  hasActiveDrop 

Instance Property

# hasActiveDrop

A Boolean value that indicates whether the table view is currently tracking a drop session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var hasActiveDrop: Bool { get }
```

## Discussion

The value of this property is true when the table view is tracking a drop session.

## See Also

### Managing drop interactions

var dropDelegate: (any UITableViewDropDelegate)?

The delegate object that manages the dropping of content into the table view.

protocol UITableViewDropDelegate

The interface for handling drops in a table view.

