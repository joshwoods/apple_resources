

- AppKit
- NSTableView
-  moveColumn(\_:toColumn:) 

Instance Method

# moveColumn(\_:toColumn:)

Moves the column and heading at the specified index to the new specified index.

macOS

``` source
@MainActor
func moveColumn(
    _ oldIndex: Int,
    toColumn newIndex: Int
)
```

## Parameters 

`oldIndex`  

The current index in the tableColumns array of the column to move.

`newIndex`  

The new index in the tableColumns array for the moved column.

## Discussion

This method posts columnDidMoveNotification to the default notification center.

## See Also

### Column Management

func addTableColumn(NSTableColumn)

Adds the specified column as the last column of the table view.

func removeTableColumn(NSTableColumn)

Removes the specified column from the table view.

var tableColumns: [NSTableColumn]

An array containing the current table column objects.

func column(withIdentifier: NSUserInterfaceItemIdentifier) -> Int

Returns the index of the first column in the table view whose identifier is equal to the specified identifier.

func tableColumn(withIdentifier: NSUserInterfaceItemIdentifier) -> NSTableColumn?

Returns the `NSTableColumn` object for the first column whose identifier is equal to the specified object.

