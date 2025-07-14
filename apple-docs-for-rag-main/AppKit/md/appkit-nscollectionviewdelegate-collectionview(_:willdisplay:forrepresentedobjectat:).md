

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:willDisplay:forRepresentedObjectAt:) 

Instance Method

# collectionView(\_:willDisplay:forRepresentedObjectAt:)

Notifies the delegate that the specified item is about to be displayed by the collection view.

macOS 10.11+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    willDisplay item: NSCollectionViewItem,
    forRepresentedObjectAt indexPath: IndexPath
)
```

## Parameters 

`collectionView`  

The collection view that is adding the item.

`item`  

The item being added.

`indexPath`  

The index path of the item.

## Discussion

The collection view calls this method before adding new items to its content. You can use this method to track the addition of items and perform related tasks.

## See Also

### Tracking the Addition and Removal of Items

func collectionView(NSCollectionView, didEndDisplaying: NSCollectionViewItem, forRepresentedObjectAt: IndexPath)

Notifies the delegate that the specified item was removed from the collection view.

func collectionView(NSCollectionView, willDisplaySupplementaryView: NSView, forElementKind: NSCollectionView.SupplementaryElementKind, at: IndexPath)

Notifies the delegate that the specified supplementary view is about to be displayed by the collection view.

func collectionView(NSCollectionView, didEndDisplayingSupplementaryView: NSView, forElementOfKind: NSCollectionView.SupplementaryElementKind, at: IndexPath)

Notifies the delegate that the specified supplementary view was removed from the collection view.

