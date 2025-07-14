

- AppKit
- NSTableView
-  highlightedTableColumn 

Instance Property

# highlightedTableColumn

The column highlighted in the table.

macOS

``` source
@MainActor
weak var highlightedTableColumn: NSTableColumn? { get set }
```

## Discussion

Assigning a value to this property highlights the specified column. A highlightable column header can be used in conjunction with row selection to highlight a particular column of the table. An example of this is how the Mail application indicates the currently sorted column.

