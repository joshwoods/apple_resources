

- AppKit
- NSTableView
-  rowSizeStyle 

Instance Property

# rowSizeStyle

The row size style (small, medium, large, or custom) used by the table view.

macOS 10.7+

``` source
@MainActor
var rowSizeStyle: NSTableView.RowSizeStyle { get set }
```

## Discussion

To set the row size style on a row by row basis, set the value of this property to NSTableView.RowSizeStyle.custom and implement the tableView(_:heightOfRow:) method in your table view delegate object.

The default value of this property is NSTableView.RowSizeStyle.custom, which tells the table to use the rowHeight of the table instead of any pre-determined system values. Generally, `rowSizeStyle` should always be NSTableView.RowSizeStyle.custom except for “source lists”.

## See Also

### Getting and Setting Row Size Styles

var effectiveRowSizeStyle: NSTableView.RowSizeStyle

The effective row size style for the table.

