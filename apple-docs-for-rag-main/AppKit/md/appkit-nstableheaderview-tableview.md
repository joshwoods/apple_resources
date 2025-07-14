

- AppKit
- NSTableHeaderView
-  tableView 

Instance Property

# tableView

The NSTableView instance that this table header view belongs to.

macOS

``` source
@MainActor
weak var tableView: NSTableView? { get set }
```

## Discussion

You should never need to set this property; it’s assigned automatically when you set the header view for an `NSTableView`.

## See Also

### Related Documentation

Table View Programming Guide for Mac

var headerView: NSTableHeaderView?

The view object used to draw headers over columns.

