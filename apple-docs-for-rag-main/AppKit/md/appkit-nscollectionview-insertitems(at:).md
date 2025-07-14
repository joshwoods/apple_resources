

- AppKit
- NSCollectionView
-  insertItems(at:) 

Instance Method

# insertItems(at:)

Inserts new items into the collection view at the specified locations.

macOS 10.11+

``` source
@MainActor
func insertItems(at indexPaths: Set)
```

## Parameters 

`indexPaths`  

A set of NSIndexPath objects, each of which includes a section and item index corresponding to the insertion point of a single item. Specifying `nil` for this parameter raises an exception.

## Discussion

After adding new items to your data source object, use this method to synchronize those changes with the collection view. Calling this method lets the collection view know that it must update its internal data structures and possibly update its visual appearance. In response, the collection view asks the layout object for information about the new objects. If the layout object indicates that the new items should appear onscreen, the collection view asks the data source to provide the appropriate content, animating that content into position as needed.

When inserting or deleting multiple sections and items, you can animate all of your changes at once using the performBatchUpdates(_:completionHandler:) method.

## See Also

### Inserting, Moving, and Deleting Items

func moveItem(at: IndexPath, to: IndexPath)

Moves an item from one location to another in the collection view.

func deleteItems(at: Set&lt;IndexPath>)

Deletes the items at the specified index paths.

