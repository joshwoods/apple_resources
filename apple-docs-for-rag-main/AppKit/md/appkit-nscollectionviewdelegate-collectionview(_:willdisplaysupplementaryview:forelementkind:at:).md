

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:willDisplaySupplementaryView:forElementKind:at:) 

Instance Method

# collectionView(\_:willDisplaySupplementaryView:forElementKind:at:)

Notifies the delegate that the specified supplementary view is about to be displayed by the collection view.

macOS 10.11+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    willDisplaySupplementaryView view: NSView,
    forElementKind elementKind: NSCollectionView.SupplementaryElementKind,
    at indexPath: IndexPath
)
```

## Parameters 

`collectionView`  

The collection view that is adding the supplementary view.

`view`  

The supplementary view being added.

`elementKind`  

The type of the supplementary view. Layouts are responsible for defining the types of supplementary views they support.

`indexPath`  

The index path associated with the supplementary view.

## Discussion

The collection view calls this method before adding new supplementary views to its content. You can use this method to track the addition of those views and perform related tasks.

## See Also

### Tracking the Addition and Removal of Items

func collectionView(NSCollectionView, willDisplay: NSCollectionViewItem, forRepresentedObjectAt: IndexPath)

Notifies the delegate that the specified item is about to be displayed by the collection view.

func collectionView(NSCollectionView, didEndDisplaying: NSCollectionViewItem, forRepresentedObjectAt: IndexPath)

Notifies the delegate that the specified item was removed from the collection view.

func collectionView(NSCollectionView, didEndDisplayingSupplementaryView: NSView, forElementOfKind: NSCollectionView.SupplementaryElementKind, at: IndexPath)

Notifies the delegate that the specified supplementary view was removed from the collection view.

