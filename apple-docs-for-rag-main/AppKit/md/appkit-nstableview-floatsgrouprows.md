

- AppKit
- NSTableView
-  floatsGroupRows 

Instance Property

# floatsGroupRows

A Boolean value indicating whether the table view draws grouped rows as if they are floating.

macOS 10.7+

``` source
@MainActor
var floatsGroupRows: Bool { get set }
```

## Discussion

Group rows are rows for which the table view delegate’s tableView(_:isGroupRow:) method returns YES. These rows can be displayed as if they are floating in a view-based table view.

The default value of this property is true.

