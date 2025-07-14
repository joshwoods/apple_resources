

- UIKit
- UICollectionView
-  insertItems(at:) 

Instance Method

# insertItems(at:)

Inserts new items at the specified index paths.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func insertItems(at indexPaths: [IndexPath])
```

## Parameters 

`indexPaths`  

An array of NSIndexPath objects, each of which contains a section index and item index at which to insert a new cell. This parameter must not be `nil`.

## Discussion

Call this method to insert one or more new items into the collection view. You might do this when your data source object receives data for new items or in response to user interactions with the collection view. The collection view gets the layout information for the new cells as part of calling this method. And if the layout information indicates that the cells should appear onscreen, the collection view asks your data source to provide the appropriate views, animating them into position as needed.

You can also call this method from a block passed to the performBatchUpdates(_:completion:) method when you want to animate multiple separate changes into place at the same time. See the description of that method for more information.

## See Also

### Inserting, moving, and deleting Items

func moveItem(at: IndexPath, to: IndexPath)

Moves an item from one location to another in the collection view.

func deleteItems(at: [IndexPath])

Deletes the items at the specified index paths.

