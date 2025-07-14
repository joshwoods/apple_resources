

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:didEndDisplaying:forRepresentedObjectAt:) 

Instance Method

# collectionView(\_:didEndDisplaying:forRepresentedObjectAt:)

Notifies the delegate that the specified item was removed from the collection view.

macOS 10.11+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    didEndDisplaying item: NSCollectionViewItem,
    forRepresentedObjectAt indexPath: IndexPath
)
```

## Parameters 

`collectionView`  

The collection view that removed the item.

`item`  

The item that was removed.

`indexPath`  

The index path of the item.

## Discussion

The collection view calls this method after removing an item from its content. You can use this method to track the removal of items and perform related tasks.

## See Also

### Tracking the Addition and Removal of Items

func collectionView(NSCollectionView, willDisplay: NSCollectionViewItem, forRepresentedObjectAt: IndexPath)

Notifies the delegate that the specified item is about to be displayed by the collection view.

func collectionView(NSCollectionView, willDisplaySupplementaryView: NSView, forElementKind: NSCollectionView.SupplementaryElementKind, at: IndexPath)

Notifies the delegate that the specified supplementary view is about to be displayed by the collection view.

func collectionView(NSCollectionView, didEndDisplayingSupplementaryView: NSView, forElementOfKind: NSCollectionView.SupplementaryElementKind, at: IndexPath)

Notifies the delegate that the specified supplementary view was removed from the collection view.

