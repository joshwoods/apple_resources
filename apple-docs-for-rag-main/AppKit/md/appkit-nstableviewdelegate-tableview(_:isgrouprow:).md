

- AppKit
- NSTableViewDelegate
-  tableView(\_:isGroupRow:) 

Instance Method

# tableView(\_:isGroupRow:)

Returns whether the specified row is a group row.

macOS 10.5+

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    isGroupRow row: Int
) -> Bool
```

## Parameters 

`tableView`  

The table view that sent the message.

`row`  

The row index.

## Return Value

true if the specified row should have the group row style drawn, false otherwise.

## Discussion

If the cell in `row` is an NSTextFieldCell object and contains only a string, the group row style attributes are automatically applied to the cell.

Group rows in NSView-based table views can be made to visually “float” by setting the table view method floatsGroupRows to true.

Note

When configured as a source list style table view, rows identified as group rows draw with a specific style unique to source lists.

## See Also

### Related Documentation

var floatsGroupRows: Bool

A Boolean value indicating whether the table view draws grouped rows as if they are floating.

