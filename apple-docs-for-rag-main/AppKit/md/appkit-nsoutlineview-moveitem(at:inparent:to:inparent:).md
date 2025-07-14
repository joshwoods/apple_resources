

- AppKit
- NSOutlineView
-  moveItem(at:inParent:to:inParent:) 

Instance Method

# moveItem(at:inParent:to:inParent:)

Moves an item at a given index in the given parent to a new index in a new parent.

macOS 10.7+

``` source
@MainActor
func moveItem(
    at fromIndex: Int,
    inParent oldParent: Any?,
    to toIndex: Int,
    inParent newParent: Any?
)
```

## Parameters 

`fromIndex`  

Index of the item to be moved.

`oldParent`  

The parent of the item to be moved.

`toIndex`  

Index in the new parent to which the item is moved.

`newParent`  

The parent of the item after it is moved.

## Discussion

This method parallels the moveRow(at:to:) method of NSTableView. The `newParent` can be the same as `oldParent` to reorder an item within the same parent.

Note

NSCell-based outline views must first call beginUpdates() before calling this method.

You can call this method multiple times within the same beginUpdates()/endUpdates() block. Moving from an invalid index, or to an invalid index, throws an exception.

## See Also

### Manipulating Items

func insertItems(at: IndexSet, inParent: Any?, withAnimation: NSTableView.AnimationOptions)

Inserts new items at the given indexes in the given parent with the specified optional animations.

func removeItems(at: IndexSet, inParent: Any?, withAnimation: NSTableView.AnimationOptions)

Removes items at the given indexes in the given parent with the specified optional animations.

