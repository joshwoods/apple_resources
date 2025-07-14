

- AppKit
- NSScrubber
-  insertItems(at:) 

Instance Method

# insertItems(at:)

Inserts new items at the specified indexes into the scrubber.

macOS 10.12.2+

``` source
@MainActor
func insertItems(at indexes: IndexSet)
```

## Parameters 

`indexes`  

An index set (IndexSet) of the indexes of the items to insert.

## Discussion

The scrubber requests the view for each index from its data source.

## See Also

### Inserting, moving, and deleting items

func moveItem(at: Int, to: Int)

Moves an item from one index to another in the scrubber.

func removeItems(at: IndexSet)

Removes the items at the specified indexes from the scrubber.

