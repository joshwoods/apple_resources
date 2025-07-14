

- AppKit
- NSCollectionView
-  moveItem(at:to:) 

Instance Method

# moveItem(at:to:)

Moves an item from one location to another in the collection view.

macOS 10.11+

``` source
@MainActor
func moveItem(
    at indexPath: IndexPath,
    to newIndexPath: IndexPath
)
```

## Parameters 

`indexPath`  

The index path of the item that you want to move. This parameter must not be `nil`.

`newIndexPath`  

The index path of the item’s new location. This parameter must not be `nil`.

## Discussion

After rearranging items in your data source object, use this method to synchronize those changes with the collection view. Calling this method lets the collection view know that it must update its internal data structures and possibly update its visual appearance. You can move the item to a different section or to a new location in the same section. The collection view updates the layout as needed to account for the move, animating cells into position in response.

When inserting or deleting multiple sections and items, you can animate all of your changes at once using the performBatchUpdates(_:completionHandler:) method.

## See Also

### Inserting, Moving, and Deleting Items

func insertItems(at: Set&lt;IndexPath>)

Inserts new items into the collection view at the specified locations.

func deleteItems(at: Set&lt;IndexPath>)

Deletes the items at the specified index paths.

