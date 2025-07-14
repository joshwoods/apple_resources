

- AppKit
- NSTableView
-  removeTableColumn(\_:) 

Instance Method

# removeTableColumn(\_:)

Removes the specified column from the table view.

macOS

``` source
@MainActor
func removeTableColumn(_ tableColumn: NSTableColumn)
```

## Parameters 

`tableColumn`  

The column to remove from the table view.

## See Also

### Related Documentation

func sizeLastColumnToFit()

Resizes the last column so the table view fits exactly within its enclosing clip view.

### Column Management

func addTableColumn(NSTableColumn)

Adds the specified column as the last column of the table view.

func moveColumn(Int, toColumn: Int)

Moves the column and heading at the specified index to the new specified index.

var tableColumns: [NSTableColumn]

An array containing the current table column objects.

func column(withIdentifier: NSUserInterfaceItemIdentifier) -> Int

Returns the index of the first column in the table view whose identifier is equal to the specified identifier.

func tableColumn(withIdentifier: NSUserInterfaceItemIdentifier) -> NSTableColumn?

Returns the `NSTableColumn` object for the first column whose identifier is equal to the specified object.

