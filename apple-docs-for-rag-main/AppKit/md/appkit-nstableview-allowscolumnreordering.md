

- AppKit
- NSTableView
-  allowsColumnReordering 

Instance Property

# allowsColumnReordering

A Boolean value indicating whether the table view allows the user to rearrange columns by dragging their headers.

macOS

``` source
@MainActor
var allowsColumnReordering: Bool { get set }
```

## Discussion

The default value of this property is true, which allows the user to rearrange the table view’s columns. You can rearrange columns programmatically regardless of this setting.

## See Also

### Related Documentation

func moveColumn(Int, toColumn: Int)

Moves the column and heading at the specified index to the new specified index.

### Configuring Behavior

var allowsColumnResizing: Bool

A Boolean value indicating whether the table view allows the user to resize columns by dragging between their headers.

var allowsMultipleSelection: Bool

A Boolean value indicating whether the table view allows the user to select more than one column or row at a time.

var allowsEmptySelection: Bool

A Boolean value indicating whether the table view allows the user to select zero columns or rows.

var allowsColumnSelection: Bool

A Boolean value indicating whether the table view allows the user to select columns by clicking their headers.

var usesAutomaticRowHeights: Bool

A Boolean value that indicates whether the table view uses autolayout to calculate the height of rows.

