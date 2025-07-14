

- AppKit
- NSTableViewDataSource
-  numberOfRows(in:) 

Instance Method

# numberOfRows(in:)

Returns the number of records managed for `aTableView` by the data source object.

macOS

``` source
@MainActor
optional func numberOfRows(in tableView: NSTableView) -> Int
```

## Parameters 

`tableView`  

The table view that sent the message.

## Return Value

The number of rows in `aTableView`.

## Discussion

An instance of NSTableView uses this method to determine how many rows it should create and display. Your numberOfRows(in:) implementation is called very frequently, so it must be efficient.

Both view-based table views and cell-based table views must implement this method.

Note

This method is mandatory unless your application is using Cocoa bindings for providing data to the table view.

## See Also

### Related Documentation

Table View Programming Guide for Mac

### Getting Values

func tableView(NSTableView, objectValueFor: NSTableColumn?, row: Int) -> Any?

Called by the table view to return the data object associated with the specified row and column.

