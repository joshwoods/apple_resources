

- AppKit
- NSTableView
-  allowsEmptySelection 

Instance Property

# allowsEmptySelection

A Boolean value indicating whether the table view allows the user to select zero columns or rows.

macOS

``` source
@MainActor
var allowsEmptySelection: Bool { get set }
```

## Discussion

The default is true, which allows the user to select zero columns or rows.

## See Also

### Related Documentation

func deselectRow(Int)

Deselects the row at the specified index if it’s selected.

func deselectColumn(Int)

Deselects the column at the specified index if it’s selected.

func deselectAll(Any?)

Deselects all selected rows or columns if empty selection is allowed; otherwise does nothing.

### Configuring Behavior

var allowsColumnReordering: Bool

A Boolean value indicating whether the table view allows the user to rearrange columns by dragging their headers.

var allowsColumnResizing: Bool

A Boolean value indicating whether the table view allows the user to resize columns by dragging between their headers.

var allowsMultipleSelection: Bool

A Boolean value indicating whether the table view allows the user to select more than one column or row at a time.

var allowsColumnSelection: Bool

A Boolean value indicating whether the table view allows the user to select columns by clicking their headers.

var usesAutomaticRowHeights: Bool

A Boolean value that indicates whether the table view uses autolayout to calculate the height of rows.

