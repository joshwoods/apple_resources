

- AppKit
- NSTableViewDataSource
-  tableView(\_:pasteboardWriterForRow:) 

Instance Method

# tableView(\_:pasteboardWriterForRow:)

Called to allow the table to support multiple item dragging.

macOS 10.7+

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    pasteboardWriterForRow row: Int
) -> (any NSPasteboardWriting)?
```

## Parameters 

`tableView`  

The table view.

`row`  

The row.

## Return Value

Returns an instance of NSPasteboardItem or a custom object that implements the NSPasteboardWriting protocol. Returning `nil` excludes the row from being dragged.

## Discussion

This method is required for multi-image dragging.

If this method is implemented, then tableView(_:writeRowsWith:to:) will not be called.

