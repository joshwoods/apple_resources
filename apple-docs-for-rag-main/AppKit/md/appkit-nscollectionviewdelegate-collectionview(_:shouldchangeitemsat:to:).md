

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:shouldChangeItemsAt:to:) 

Instance Method

# collectionView(\_:shouldChangeItemsAt:to:)

Asks the delegate to approve the pending highlighting of the specified items.

macOS 10.11+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    shouldChangeItemsAt indexPaths: Set,
    to highlightState: NSCollectionViewItem.HighlightState
) -> Set
```

## Parameters 

`collectionView`  

The collection view making the request.

`indexPaths`  

The set of NSIndexPath objects corresponding to the items being highlighted.

`highlightState`  

The new highlight state for the items.

## Return Value

The set of NSIndexPath objects corresponding to the items that you want to receive the specified highlight. If you do not want any items to receive the specified highlight state, return an empty set.

## Discussion

Use this method to approve or modify the set of items targeted to receive the specified highlight state. During interactive selection or dragging, the collection view calls this method when actions occur that would affect the highlight state of items. Your implementation of the method can return the proposed set of index paths as-is or modify the set and disallow the highlighting of some or all of the items. Removing items from the set suppresses the corresponding actions, such as selecting the item or showing its eligibility as a drop target.

If you do not implement this method, the collection view updates the highlight state for the items specified by the `indexPaths` parameter.

## See Also

### Managing Item Highlighting

func collectionView(NSCollectionView, didChangeItemsAt: Set&lt;IndexPath>, to: NSCollectionViewItem.HighlightState)

Notifies the delegate that the highlight state of the specified items changed.

