

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:didChangeItemsAt:to:) 

Instance Method

# collectionView(\_:didChangeItemsAt:to:)

Notifies the delegate that the highlight state of the specified items changed.

macOS 10.11+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    didChangeItemsAt indexPaths: Set,
    to highlightState: NSCollectionViewItem.HighlightState
)
```

## Parameters 

`collectionView`  

The collection view notifying you of the highlight change.

`indexPaths`  

The set of NSIndexPath objects corresponding to the items whose highlight state changed.

`highlightState`  

The new highlight state of the items.

## Discussion

After the highlight state of one or more items changes successfully, the collection view calls this method to report the change. Use this method to respond to the change and to make any necessary adjustments to your content or the collection view.

## See Also

### Managing Item Highlighting

func collectionView(NSCollectionView, shouldChangeItemsAt: Set&lt;IndexPath>, to: NSCollectionViewItem.HighlightState) -> Set&lt;IndexPath>

Asks the delegate to approve the pending highlighting of the specified items.

