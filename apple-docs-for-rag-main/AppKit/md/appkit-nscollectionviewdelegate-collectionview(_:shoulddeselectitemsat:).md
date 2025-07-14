

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:shouldDeselectItemsAt:) 

Instance Method

# collectionView(\_:shouldDeselectItemsAt:)

Asks the delegate object to approve the pending deselection of items.

macOS 10.11+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    shouldDeselectItemsAt indexPaths: Set
) -> Set
```

## Parameters 

`collectionView`  

The collection view making the request.

`indexPaths`  

The set of NSIndexPath objects corresponding to the items deselected by the user.

## Return Value

The set of NSIndexPath objects corresponding to the items that you want to be deselected. If you do not want any items deselected, return an empty set.

## Discussion

Use this method to approve or modify the items that the user tries to deselect. During interactive selection, the collection view calls this method whenever the user deselects items. Your implementation of the method can return the proposed set of index paths as-is or modify the set before returning it. You might modify the set to disallow the deselection of specific items.

This method is not called when you set the selection programmatically using the methods of the NSCollectionView class. If you do not implement this method, the collection view deselects the items specified by the `indexPaths` parameter.

## See Also

### Managing the Selection

func collectionView(NSCollectionView, shouldSelectItemsAt: Set&lt;IndexPath>) -> Set&lt;IndexPath>

Asks the delegate to approve the pending selection of items.

func collectionView(NSCollectionView, didSelectItemsAt: Set&lt;IndexPath>)

Notifies the delegate object that one or more items were selected.

func collectionView(NSCollectionView, didDeselectItemsAt: Set&lt;IndexPath>)

Notifies the delegate object that one or more items were deselected.

