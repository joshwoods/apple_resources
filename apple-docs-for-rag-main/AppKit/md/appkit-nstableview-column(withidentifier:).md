

- AppKit
- NSTableView
-  column(withIdentifier:) 

Instance Method

# column(withIdentifier:)

Returns the index of the first column in the table view whose identifier is equal to the specified identifier.

macOS

``` source
@MainActor
func column(withIdentifier identifier: NSUserInterfaceItemIdentifier) -> Int
```

## Parameters 

`identifier`  

A column identifier.

## Return Value

The index in the tableColumns array of the first column in the table view whose identifier is equal to `anObject` (when compared using `isEqual:`), or `–1` if no columns are found with the specified identifier.

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

func tableColumn(withIdentifier: NSUserInterfaceItemIdentifier) -> NSTableColumn?

Returns the `NSTableColumn` object for the first column whose identifier is equal to the specified object.

