

- UIKit
- UITableViewDropCoordinator
-  drop(\_:to:) 

Instance Method

# drop(\_:to:)

Animates the item to the specified location and inserts a placeholder cell at that location.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func drop(
    _ dragItem: UIDragItem,
    to placeholder: UITableViewDropPlaceholder
) -> any UITableViewDropPlaceholderContext
```

**Required**

## Parameters 

`dragItem`  

The drag item containing the data to drop.

`placeholder`  

The object that contains information about the type of placeholder cell to insert, and where to insert it.

## Return Value

The context object that you use to replace or remove the placeholder cell later. Store a reference to this object so that you can call its methods later.

## Discussion

Use this method to insert a temporary placeholder cell (instead of a cell backed by actual data) into the table view. When calling this method, do not update your data source object to account for the placeholder. The table view manages the placeholder until you explicitly remove it using the returned context object.

Typically, you use this method when you must load data asynchronously for a cell. Instead of updating your data source, you insert a placeholder cell. When the data is finally available, update your data source object and call the commitInsertion(dataSourceUpdates:) method of the returned context object to swap out the placeholder cell for an actual cell. You can also remove a placeholder cell that is no longer needed by calling the deletePlaceholder() method.

At some point after calling this method, the table view executes the cellUpdateHandler block in the provided `placeholder` object. Use that block to configure the contents of the placeholder cell.

## See Also

### Animating rows to their destination

func drop(UIDragItem, toRowAt: IndexPath) -> any UIDragAnimating

Animates the item to the specified index path in the table view.

**Required**

func drop(UIDragItem, intoRowAt: IndexPath, rect: CGRect) -> any UIDragAnimating

**Required**

func drop(UIDragItem, to: UIDragPreviewTarget) -> any UIDragAnimating

Animates the item to an arbitrary location in your view hierarchy.

**Required**

