

- AppKit
- NSTableView
-  tableColumns 

Instance Property

# tableColumns

An array containing the current table column objects.

macOS

``` source
@MainActor
var tableColumns: [NSTableColumn] { get }
```

## Discussion

This property contains an array of NSTableColumn objects corresponding to the columns in the table. This array contains all columns, including those that are currently hidden.

## See Also

### Column Management

func addTableColumn(NSTableColumn)

Adds the specified column as the last column of the table view.

func removeTableColumn(NSTableColumn)

Removes the specified column from the table view.

func moveColumn(Int, toColumn: Int)

Moves the column and heading at the specified index to the new specified index.

func column(withIdentifier: NSUserInterfaceItemIdentifier) -> Int

Returns the index of the first column in the table view whose identifier is equal to the specified identifier.

func tableColumn(withIdentifier: NSUserInterfaceItemIdentifier) -> NSTableColumn?

Returns the `NSTableColumn` object for the first column whose identifier is equal to the specified object.

