

- AppKit
- NSTableView
-  headerView 

Instance Property

# headerView

The view object used to draw headers over columns.

macOS

``` source
@MainActor
var headerView: NSTableHeaderView? { get set }
```

## Discussion

To configure a table without a header view or to remove the table view’s current header view, set the value of this property to `nil`. For more information about header views, see NSTableHeaderView.

## See Also

### Setting Auxiliary Views

var cornerView: NSView?

The view used to draw the area to the right of the column headers and above the vertical scroller of the enclosing scroll view.

