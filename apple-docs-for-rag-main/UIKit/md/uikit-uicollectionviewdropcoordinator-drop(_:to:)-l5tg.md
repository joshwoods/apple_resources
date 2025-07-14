

- UIKit
- UICollectionViewDropCoordinator
-  drop(\_:to:) 

Instance Method

# drop(\_:to:)

Animates the item to the specified location and inserts a placeholder cell at that location.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func drop(
    _ dragItem: UIDragItem,
    to placeholder: UICollectionViewDropPlaceholder
) -> any UICollectionViewDropPlaceholderContext
```

**Required**

## Parameters 

`dragItem`  

The drag item containing the data to drop.

`placeholder`  

The placeholder to add at the specified location.

## Return Value

The context object that you use to replace or remove the placeholder cell later. Store a reference to this object so that you can call its methods later.

## Mentioned in 

Supporting Drag and Drop in Collection Views

## Discussion

Use this method to insert a temporary placeholder cell (instead of a cell backed by actual data) into the collection view. When calling this method, don’t update your data source object to account for the placeholder. The collection view manages the placeholder until you explicitly remove it using the returned context object.

Typically, you use this method when you must load data asynchronously for a cell. Instead of updating your data source, you insert a placeholder cell. When the data is finally available, update your data source object and call the commitInsertion(dataSourceUpdates:) method of the returned context object to swap out the placeholder cell for an actual cell. You can also remove a placeholder cell that’s no longer needed by calling the deletePlaceholder() method.

At some point after calling this method, the collection view executes your `cellUpdateHandler` block. Use that block to configure the contents of the placeholder cell. Calling the setNeedsCellUpdate() method of the returned context object executes your handler again, giving you a way to update the cell later.

## See Also

### Animating Items to Their Destination

func drop(UIDragItem, toItemAt: IndexPath) -> any UIDragAnimating

Animates the item to the specified index path in the collection view.

**Required**

func drop(UIDragItem, intoItemAt: IndexPath, rect: CGRect) -> any UIDragAnimating

Animates the item to the specified rectangle in the collection view.

**Required**

func drop(UIDragItem, to: UIDragPreviewTarget) -> any UIDragAnimating

Animates the item to an arbitrary location in your view hierarchy.

**Required**

