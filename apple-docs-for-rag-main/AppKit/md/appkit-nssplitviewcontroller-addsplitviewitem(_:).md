

- AppKit
- NSSplitViewController
-  addSplitViewItem(\_:) 

Instance Method

# addSplitViewItem(\_:)

Adds a split view item to the end of the array of split view items.

macOS 10.10+

``` source
@MainActor
func addSplitViewItem(_ splitViewItem: NSSplitViewItem)
```

## Parameters 

`splitViewItem`  

The split view item to add.

Important

Before you add a split view item, it must be non-`nil` and it must have an associated view controller, or the system throws an exception.

## Discussion

This is a convenience method you can use in place of the insertSplitViewItem(_:at:) method when you want to add a split view item to the end of the splitViewItems array. Calling this method implicitly calls the insertSplitViewItem(_:at:) method.

If you subclass the NSSplitViewController class, don’t call this method in your custom object to add a split view item. Instead, call the insertSplitViewItem(_:at:) method directly.

## See Also

### Modifying a Split View Controller

func insertSplitViewItem(NSSplitViewItem, at: Int)

Adds a split view item to the array of split view items at the specified index position.

func removeSplitViewItem(NSSplitViewItem)

Removes a specified split view item from the split view controller.

