

- AppKit
- NSScrubber
-  moveItem(at:to:) 

Instance Method

# moveItem(at:to:)

Moves an item from one index to another in the scrubber.

macOS 10.12.2+

``` source
@MainActor
func moveItem(
    at oldIndex: Int,
    to newIndex: Int
)
```

## Parameters 

`oldIndex`  

The index of the item that you want to move.

`newIndex`  

The index of the item’s new location.

## See Also

### Inserting, moving, and deleting items

func insertItems(at: IndexSet)

Inserts new items at the specified indexes into the scrubber.

func removeItems(at: IndexSet)

Removes the items at the specified indexes from the scrubber.

