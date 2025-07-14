

- AppKit
- NSSplitViewController
-  removeSplitViewItem(\_:) 

Instance Method

# removeSplitViewItem(\_:)

Removes a specified split view item from the split view controller.

macOS 10.10+

``` source
@MainActor
func removeSplitViewItem(_ splitViewItem: NSSplitViewItem)
```

## Parameters 

`splitViewItem`  

The split view item to remove.

Important

If the split view item is `nil` or isn’t in the splitViewItems array, the system throws an exception.

## Discussion

After you remove a split view item, the system adjusts the layout of the split view accordingly.

## See Also

### Modifying a Split View Controller

func addSplitViewItem(NSSplitViewItem)

Adds a split view item to the end of the array of split view items.

func insertSplitViewItem(NSSplitViewItem, at: Int)

Adds a split view item to the array of split view items at the specified index position.

