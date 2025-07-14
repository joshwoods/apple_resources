

- AppKit
- NSTableViewDelegate
-  tableView(\_:shouldEdit:row:) 

Instance Method

# tableView(\_:shouldEdit:row:)

Asks the delegate if the cell at the specified row and column can be edited.

macOS

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    shouldEdit tableColumn: NSTableColumn?,
    row: Int
) -> Bool
```

## Parameters 

`tableView`  

The table view that sent the message.

`tableColumn`  

The table column.

`row`  

The row index.

## Return Value

true to allow editing the cell, false to deny editing.

## Discussion

The delegate can implement this method to disallow editing of specific cells.

Note

This method is only valid for NSCell-based table views.

