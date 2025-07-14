

- AppKit
- NSTableViewDataSource
-  tableView(\_:objectValueFor:row:) 

Instance Method

# tableView(\_:objectValueFor:row:)

Called by the table view to return the data object associated with the specified row and column.

macOS

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    objectValueFor tableColumn: NSTableColumn?,
    row: Int
) -> Any?
```

## Parameters 

`tableView`  

The table view that sent the message.

`tableColumn`  

A column in `aTableView`.

`row`  

The row of the item in `aTableColumn`.

## Return Value

An item in the data source in the specified table column of the view.

## Discussion

tableView(_:objectValueFor:row:) is called each time the table cell needs to be redisplayed, so it must be efficient.

Note

This method is mandatory unless your application is using Cocoa bindings for providing data to the table view.

## See Also

### Getting Values

func numberOfRows(in: NSTableView) -> Int

Returns the number of records managed for `aTableView` by the data source object.

