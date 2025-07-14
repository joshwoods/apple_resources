

- AppKit
- NSTableView
-  allowsColumnResizing 

Instance Property

# allowsColumnResizing

A Boolean value indicating whether the table view allows the user to resize columns by dragging between their headers.

macOS

``` source
@MainActor
var allowsColumnResizing: Bool { get set }
```

## Discussion

The default of this property is true, which allows the user to resize the table view’s columns. You can resize columns programmatically regardless of this setting.

## See Also

### Related Documentation

var width: CGFloat

The table column’s width, in points.

### Configuring Behavior

var allowsColumnReordering: Bool

A Boolean value indicating whether the table view allows the user to rearrange columns by dragging their headers.

var allowsMultipleSelection: Bool

A Boolean value indicating whether the table view allows the user to select more than one column or row at a time.

var allowsEmptySelection: Bool

A Boolean value indicating whether the table view allows the user to select zero columns or rows.

var allowsColumnSelection: Bool

A Boolean value indicating whether the table view allows the user to select columns by clicking their headers.

var usesAutomaticRowHeights: Bool

A Boolean value that indicates whether the table view uses autolayout to calculate the height of rows.

