

- AppKit
- NSTableView
-  addTableColumn(\_:) 

Instance Method

# addTableColumn(\_:)

Adds the specified column as the last column of the table view.

macOS

``` source
@MainActor
func addTableColumn(_ tableColumn: NSTableColumn)
```

## Parameters 

`tableColumn`  

The column to add to the table view.

## See Also

### Related Documentation

func sizeLastColumnToFit()

Resizes the last column so the table view fits exactly within its enclosing clip view.

### Column Management

func removeTableColumn(NSTableColumn)

Removes the specified column from the table view.

func moveColumn(Int, toColumn: Int)

Moves the column and heading at the specified index to the new specified index.

var tableColumns: [NSTableColumn]

An array containing the current table column objects.

func column(withIdentifier: NSUserInterfaceItemIdentifier) -> Int

Returns the index of the first column in the table view whose identifier is equal to the specified identifier.

func tableColumn(withIdentifier: NSUserInterfaceItemIdentifier) -> NSTableColumn?

Returns the `NSTableColumn` object for the first column whose identifier is equal to the specified object.

