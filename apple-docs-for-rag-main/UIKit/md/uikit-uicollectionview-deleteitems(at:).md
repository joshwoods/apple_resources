

- UIKit
- UICollectionView
-  deleteItems(at:) 

Instance Method

# deleteItems(at:)

Deletes the items at the specified index paths.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func deleteItems(at indexPaths: [IndexPath])
```

## Parameters 

`indexPaths`  

An array of NSIndexPath objects, each of which contains a section index and item index for the item you want to delete from the collection view. This parameter must not be `nil`.

## Discussion

Use this method to remove items from the collection view. You might do this when you remove the items from your data source object or in response to user interactions with the collection view. The collection view updates the layout of the remaining items to account for the deletions, animating the remaining items into position as needed.

You can also call this method from a block passed to the performBatchUpdates(_:completion:) method when you want to animate multiple separate changes into place at the same time. See the description of that method for more information.

## See Also

### Inserting, moving, and deleting Items

func insertItems(at: [IndexPath])

Inserts new items at the specified index paths.

func moveItem(at: IndexPath, to: IndexPath)

Moves an item from one location to another in the collection view.

