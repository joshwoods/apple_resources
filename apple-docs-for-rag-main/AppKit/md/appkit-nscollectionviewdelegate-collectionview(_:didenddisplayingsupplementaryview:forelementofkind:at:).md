

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:didEndDisplayingSupplementaryView:forElementOfKind:at:) 

Instance Method

# collectionView(\_:didEndDisplayingSupplementaryView:forElementOfKind:at:)

Notifies the delegate that the specified supplementary view was removed from the collection view.

macOS 10.11+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    didEndDisplayingSupplementaryView view: NSView,
    forElementOfKind elementKind: NSCollectionView.SupplementaryElementKind,
    at indexPath: IndexPath
)
```

## Parameters 

`collectionView`  

The collection view that removed the view.

`view`  

The supplementary view that was removed.

`elementKind`  

The type of the supplementary view. Layouts are responsible for defining the types of supplementary views they support.

`indexPath`  

The index path associated with the supplementary view.

## Discussion

The collection view calls this method after removing a supplementary view from its content. You can use this method to track the removal of views and perform related tasks.

## See Also

### Tracking the Addition and Removal of Items

func collectionView(NSCollectionView, willDisplay: NSCollectionViewItem, forRepresentedObjectAt: IndexPath)

Notifies the delegate that the specified item is about to be displayed by the collection view.

func collectionView(NSCollectionView, didEndDisplaying: NSCollectionViewItem, forRepresentedObjectAt: IndexPath)

Notifies the delegate that the specified item was removed from the collection view.

func collectionView(NSCollectionView, willDisplaySupplementaryView: NSView, forElementKind: NSCollectionView.SupplementaryElementKind, at: IndexPath)

Notifies the delegate that the specified supplementary view is about to be displayed by the collection view.

