

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:didEndDisplayingSupplementaryView:forElementOfKind:at:) 

Instance Method

# collectionView(\_:didEndDisplayingSupplementaryView:forElementOfKind:at:)

Tells the delegate that the specified supplementary view was removed from the collection view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    didEndDisplayingSupplementaryView view: UICollectionReusableView,
    forElementOfKind elementKind: String,
    at indexPath: IndexPath
)
```

## Parameters 

`collectionView`  

The collection view object that removed the supplementary view.

`view`  

The view that was removed.

`elementKind`  

The type of the supplementary view. This string is defined by the layout that presents the view.

`indexPath`  

The index path of the data item that the supplementary view represented.

## Discussion

Use this method to detect when a supplementary view is removed from a collection view, as opposed to monitoring the view itself to see when it appears or disappears.

## See Also

### Tracking the addition and removal of views

func collectionView(UICollectionView, willDisplay: UICollectionViewCell, forItemAt: IndexPath)

Tells the delegate that the specified cell is about to be displayed in the collection view.

func collectionView(UICollectionView, willDisplaySupplementaryView: UICollectionReusableView, forElementKind: String, at: IndexPath)

Tells the delegate that the specified supplementary view is about to be displayed in the collection view.

func collectionView(UICollectionView, didEndDisplaying: UICollectionViewCell, forItemAt: IndexPath)

Tells the delegate that the specified cell was removed from the collection view.

