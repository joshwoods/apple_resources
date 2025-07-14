

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:shouldSelectItemsAt:) 

Instance Method

# collectionView(\_:shouldSelectItemsAt:)

Asks the delegate to approve the pending selection of items.

macOS 10.11+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    shouldSelectItemsAt indexPaths: Set
) -> Set
```

## Parameters 

`collectionView`  

The collection view making the request.

`indexPaths`  

The set of NSIndexPath objects corresponding to the items selected by the user.

## Return Value

The set of NSIndexPath objects corresponding to the items that you want to be selected. If you do not want any items selected, return an empty set.

## Discussion

Use this method to approve or modify the items that the user tries to select. During interactive selection, the collection view calls this method whenever the user selects new items. Your implementation of the method can return the proposed set of index paths as-is or modify the set before returning it. You might modify the set to disallow the selection of specific items or specific combinations of items.

This method is not called when you set the selection programmatically using the methods of the NSCollectionView class. If you do not implement this method, the collection view selects the items specified by the `indexPaths` parameter.

## See Also

### Managing the Selection

func collectionView(NSCollectionView, didSelectItemsAt: Set&lt;IndexPath>)

Notifies the delegate object that one or more items were selected.

func collectionView(NSCollectionView, shouldDeselectItemsAt: Set&lt;IndexPath>) -> Set&lt;IndexPath>

Asks the delegate object to approve the pending deselection of items.

func collectionView(NSCollectionView, didDeselectItemsAt: Set&lt;IndexPath>)

Notifies the delegate object that one or more items were deselected.

