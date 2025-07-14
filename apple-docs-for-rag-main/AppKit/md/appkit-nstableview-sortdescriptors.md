

- AppKit
- NSTableView
-  sortDescriptors 

Instance Property

# sortDescriptors

The table view’s sort descriptors.

macOS

``` source
@MainActor
var sortDescriptors: [NSSortDescriptor] { get set }
```

## Discussion

This property contains an array of NSSortDescriptor objects. A table column is considered sortable if it has a sort descriptor that specifies the sorting direction, a key to sort by, and a selector defining how to sort. Changing the value of this property may have the side effect of calling the tableView(_:sortDescriptorsDidChange:) method on the table view’s data source.

The contents of this property are archived and persisted along with other column information if autosave is enabled for the table.

