

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:willDisplaySupplementaryView:forElementKind:at:) 

Instance Method

# collectionView(\_:willDisplaySupplementaryView:forElementKind:at:)

Tells the delegate that the specified supplementary view is about to be displayed in the collection view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    willDisplaySupplementaryView view: UICollectionReusableView,
    forElementKind elementKind: String,
    at indexPath: IndexPath
)
```

## Parameters 

`collectionView`  

The collection view object that is adding the supplementary view.

`view`  

The view being added.

`elementKind`  

The type of the supplementary view. This string is defined by the layout that presents the view.

`indexPath`  

The index path of the data item that the supplementary view represents.

## Discussion

The collection view calls this method before adding a supplementary view to its content. Use this method to detect view additions, as opposed to monitoring the view itself to see when it appears.

## See Also

### Tracking the addition and removal of views

func collectionView(UICollectionView, willDisplay: UICollectionViewCell, forItemAt: IndexPath)

Tells the delegate that the specified cell is about to be displayed in the collection view.

func collectionView(UICollectionView, didEndDisplaying: UICollectionViewCell, forItemAt: IndexPath)

Tells the delegate that the specified cell was removed from the collection view.

func collectionView(UICollectionView, didEndDisplayingSupplementaryView: UICollectionReusableView, forElementOfKind: String, at: IndexPath)

Tells the delegate that the specified supplementary view was removed from the collection view.

