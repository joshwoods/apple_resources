

- AppKit
- NSTableView
-  allowsMultipleSelection 

Instance Property

# allowsMultipleSelection

A Boolean value indicating whether the table view allows the user to select more than one column or row at a time.

macOS

``` source
@MainActor
var allowsMultipleSelection: Bool { get set }
```

## Discussion

The default is false, which allows the user to select only one column or row at a time. You can select multiple columns or rows programmatically regardless of this setting.

## See Also

### Related Documentation

func selectColumnIndexes(IndexSet, byExtendingSelection: Bool)

Sets the column selection using `indexes` possibly extending the selection.

func selectRowIndexes(IndexSet, byExtendingSelection: Bool)

Sets the row selection using `indexes` extending the selection if specified.

### Configuring Behavior

var allowsColumnReordering: Bool

A Boolean value indicating whether the table view allows the user to rearrange columns by dragging their headers.

var allowsColumnResizing: Bool

A Boolean value indicating whether the table view allows the user to resize columns by dragging between their headers.

var allowsEmptySelection: Bool

A Boolean value indicating whether the table view allows the user to select zero columns or rows.

var allowsColumnSelection: Bool

A Boolean value indicating whether the table view allows the user to select columns by clicking their headers.

var usesAutomaticRowHeights: Bool

A Boolean value that indicates whether the table view uses autolayout to calculate the height of rows.

