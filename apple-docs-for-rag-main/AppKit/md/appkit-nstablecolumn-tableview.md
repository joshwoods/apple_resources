

- AppKit
- NSTableColumn
-  tableView 

Instance Property

# tableView

The table view that contains the table column.

macOS

``` source
@MainActor
weak var tableView: NSTableView? { get set }
```

## Discussion

You should never need to set this property; it’s set automatically when you add a table column to a table view using the `NSTableView` class’s method addTableColumn(_:).

## See Also

### Related Documentation

func addTableColumn(NSTableColumn)

Adds the specified column as the last column of the table view.

