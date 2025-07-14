

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:didDeselectItemsAt:) 

Instance Method

# collectionView(\_:didDeselectItemsAt:)

Notifies the delegate object that one or more items were deselected.

macOS 10.11+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    didDeselectItemsAt indexPaths: Set
)
```

## Parameters 

`collectionView`  

The collection view notifying you of the selection change.

`indexPaths`  

The set of NSIndexPath objects corresponding to the items that were deselected.

## Discussion

After the user successfully deselects one or more items, the collection view calls this method to let you know that the items are no longer selected. Use this method to respond to the selection change and to make any necessary adjustments to your content or the collection view.

This method is not called when you set the selection programmatically using the methods of the NSCollectionView class.

## See Also

### Managing the Selection

func collectionView(NSCollectionView, shouldSelectItemsAt: Set&lt;IndexPath>) -> Set&lt;IndexPath>

Asks the delegate to approve the pending selection of items.

func collectionView(NSCollectionView, didSelectItemsAt: Set&lt;IndexPath>)

Notifies the delegate object that one or more items were selected.

func collectionView(NSCollectionView, shouldDeselectItemsAt: Set&lt;IndexPath>) -> Set&lt;IndexPath>

Asks the delegate object to approve the pending deselection of items.

