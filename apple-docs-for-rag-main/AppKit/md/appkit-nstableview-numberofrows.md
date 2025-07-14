

- AppKit
- NSTableView
-  numberOfRows 

Instance Property

# numberOfRows

The number of rows in the table.

macOS

``` source
@MainActor
var numberOfRows: Int { get }
```

## Discussion

Typically you should not ask the table view how many rows it has; instead, interrogate the table view’s data source.

## See Also

### Related Documentation

func numberOfRows(in: NSTableView) -> Int

Returns the number of records managed for `aTableView` by the data source object.

### Table Dimensions

var numberOfColumns: Int

The number of columns in the table.

