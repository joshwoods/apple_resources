

- AppKit
- NSTableView
-  tableColumn(withIdentifier:) 

Instance Method

# tableColumn(withIdentifier:)

Returns the `NSTableColumn` object for the first column whose identifier is equal to the specified object.

macOS

``` source
@MainActor
func tableColumn(withIdentifier identifier: NSUserInterfaceItemIdentifier) -> NSTableColumn?
```

## Parameters 

`identifier`  

A column identifier.

## Return Value

The `NSTableColumn` object for the first column whose identifier is equal to `anObject` (when compared using `isEqual:`), or `nil` if no columns are found with the specified identifier.

## See Also

### Column Management

func addTableColumn(NSTableColumn)

Adds the specified column as the last column of the table view.

func removeTableColumn(NSTableColumn)

Removes the specified column from the table view.

func moveColumn(Int, toColumn: Int)

Moves the column and heading at the specified index to the new specified index.

var tableColumns: [NSTableColumn]

An array containing the current table column objects.

func column(withIdentifier: NSUserInterfaceItemIdentifier) -> Int

Returns the index of the first column in the table view whose identifier is equal to the specified identifier.

