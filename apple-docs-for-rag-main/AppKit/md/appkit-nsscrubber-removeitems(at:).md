

- AppKit
- NSScrubber
-  removeItems(at:) 

Instance Method

# removeItems(at:)

Removes the items at the specified indexes from the scrubber.

macOS 10.12.2+

``` source
@MainActor
func removeItems(at indexes: IndexSet)
```

## Parameters 

`indexes`  

An index set (IndexSet) of the indexes of the items to remove.

## See Also

### Inserting, moving, and deleting items

func insertItems(at: IndexSet)

Inserts new items at the specified indexes into the scrubber.

func moveItem(at: Int, to: Int)

Moves an item from one index to another in the scrubber.

