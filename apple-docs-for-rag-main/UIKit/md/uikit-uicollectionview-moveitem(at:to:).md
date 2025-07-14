

- UIKit
- UICollectionView
-  moveItem(at:to:) 

Instance Method

# moveItem(at:to:)

Moves an item from one location to another in the collection view.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func moveItem(
    at indexPath: IndexPath,
    to newIndexPath: IndexPath
)
```

## Parameters 

`indexPath`  

The index path of the item you want to move. This parameter must not be `nil`.

`newIndexPath`  

The index path of the item’s new location. This parameter must not be `nil`.

## Discussion

Use this method to reorganize existing data items. You might do this when you rearrange the items within your data source object or in response to user interactions with the collection view. You can move items between sections or within the same section. The collection view updates the layout as needed to account for the move, animating cells into position as needed.

You can also call this method from a block passed to the performBatchUpdates(_:completion:) method when you want to animate multiple separate changes into place at the same time. See the description of that method for more information.

## See Also

### Inserting, moving, and deleting Items

func insertItems(at: [IndexPath])

Inserts new items at the specified index paths.

func deleteItems(at: [IndexPath])

Deletes the items at the specified index paths.

