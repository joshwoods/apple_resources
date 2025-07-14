

- AppKit
- NSTableColumn
-  dataCell Deprecated

Instance Property

# dataCell

The cell prototype used by the table column to draw individual cells.

macOS

``` source
@MainActor
var dataCell: Any { get set }
```

Deprecated

Cell-based table views are deprecated; use view-based table views instead. See tableView(_:viewFor:row:) and view(atColumn:row:makeIfNecessary:).

## Discussion

You can use this property to control the font, alignment, and other text attributes for the table column contents.

You can also assign a cell that displays things other than text—for example, you can display images by setting the cell to NSImageCell.

Note

This property is only valid for cell-based table views.

## See Also

### Deprecated Methods

func dataCell(forRow: Int) -> Any

Returns the cell object used to display values in the specified row of the table column.

Deprecated

