

- AppKit
- NSTableCellView
-  objectValue 

Instance Property

# objectValue

The object that represents the cell data.

macOS 10.7+

``` source
@MainActor
var objectValue: Any? { get set }
```

## Discussion

The `objectValue` is automatically set by the table when using bindings or is the object returned by the NSTableViewDataSource protocol method tableView(_:objectValueFor:row:).

## See Also

### Related Documentation

func tableView(NSTableView, objectValueFor: NSTableColumn?, row: Int) -> Any?

Called by the table view to return the data object associated with the specified row and column.

Drag and Drop Programming Topics

Table View Programming Guide for Mac

