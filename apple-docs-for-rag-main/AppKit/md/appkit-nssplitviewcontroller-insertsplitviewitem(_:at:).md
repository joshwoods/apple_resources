

- AppKit
- NSSplitViewController
-  insertSplitViewItem(\_:at:) 

Instance Method

# insertSplitViewItem(\_:at:)

Adds a split view item to the array of split view items at the specified index position.

macOS 10.10+

``` source
@MainActor
func insertSplitViewItem(
    _ splitViewItem: NSSplitViewItem,
    at index: Int
)
```

## Parameters 

`splitViewItem`  

The split view item to add.

Important

Before you add a split view item, it must be non-`nil` and it must have an associated view controller, or the system throws an exception.

`index`  

The index position for adding the split view item in the splitViewItems array.

Important

If the index value is out of bounds (less than `0` or greater than the count of the array), the system throws an exception.

## Discussion

If the split view controller’s view finishes loading, and the split view item that you add is visible, the system loads the split view item’s view controller’s view and adds it to the split view.

## See Also

### Modifying a Split View Controller

func addSplitViewItem(NSSplitViewItem)

Adds a split view item to the end of the array of split view items.

func removeSplitViewItem(NSSplitViewItem)

Removes a specified split view item from the split view controller.

