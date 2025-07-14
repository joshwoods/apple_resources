

- AppKit
- NSOutlineView
-  insertItems(at:inParent:withAnimation:) 

Instance Method

# insertItems(at:inParent:withAnimation:)

Inserts new items at the given indexes in the given parent with the specified optional animations.

macOS 10.7+

``` source
@MainActor
func insertItems(
    at indexes: IndexSet,
    inParent parent: Any?,
    withAnimation animationOptions: NSTableView.AnimationOptions = []
)
```

## Parameters 

`indexes`  

Indexes at which to insert items.

`parent`  

The parent for the items, or `nil` if the parent is the root.

`animationOptions`  

Animated slide effects used when inserting items.

## Discussion

This method parallels the insertRows(at:withAnimation:) method of NSTableView and is used in a way similar to the insert(_:at:) method of NSMutableArray. The method does nothing if `parent` is not expanded. The actual item values are determined by the data source’s outlineView(_:child:ofItem:) method (which is called only after endUpdates() to ensure data source integrity).

Note

NSCell-based outline views must first call beginUpdates() before calling this method.

You can call this method multiple times within the same beginUpdates()/endUpdates() block; new insertions move previously inserted new items, just like modifying an array. Inserting an index beyond what is available throws an exception.

## See Also

### Manipulating Items

func moveItem(at: Int, inParent: Any?, to: Int, inParent: Any?)

Moves an item at a given index in the given parent to a new index in a new parent.

func removeItems(at: IndexSet, inParent: Any?, withAnimation: NSTableView.AnimationOptions)

Removes items at the given indexes in the given parent with the specified optional animations.

