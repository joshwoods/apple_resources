

- AppKit
- NSOutlineView
-  removeItems(at:inParent:withAnimation:) 

Instance Method

# removeItems(at:inParent:withAnimation:)

Removes items at the given indexes in the given parent with the specified optional animations.

macOS 10.7+

``` source
@MainActor
func removeItems(
    at indexes: IndexSet,
    inParent parent: Any?,
    withAnimation animationOptions: NSTableView.AnimationOptions = []
)
```

## Parameters 

`indexes`  

Indexes of the items to be removed.

`parent`  

The parent of the items to be removed.

`animationOptions`  

Animated slide effects used when removing items.

## Discussion

This method parallels the removeRows(at:withAnimation:) method of NSTableView and is used in a way similar to the removeObjects(at:) method of NSMutableArray. The method does nothing if `parent` is not expanded. If any of the child items is expanded, then all of its child rows are also be removed.

Note

NSCell-based outline views must first call beginUpdates() before calling this method.

You can call this method multiple times within the same beginUpdates()/endUpdates() block; changes work just like modifying an array. Removing an item at an index beyond what is available throws an exception.

## See Also

### Manipulating Items

func insertItems(at: IndexSet, inParent: Any?, withAnimation: NSTableView.AnimationOptions)

Inserts new items at the given indexes in the given parent with the specified optional animations.

func moveItem(at: Int, inParent: Any?, to: Int, inParent: Any?)

Moves an item at a given index in the given parent to a new index in a new parent.

