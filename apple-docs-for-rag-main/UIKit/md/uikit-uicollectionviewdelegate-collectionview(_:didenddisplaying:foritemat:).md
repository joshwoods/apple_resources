

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:didEndDisplaying:forItemAt:) 

Instance Method

# collectionView(\_:didEndDisplaying:forItemAt:)

Tells the delegate that the specified cell was removed from the collection view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    didEndDisplaying cell: UICollectionViewCell,
    forItemAt indexPath: IndexPath
)
```

## Parameters 

`collectionView`  

The collection view object that removed the cell.

`cell`  

The cell object that was removed.

`indexPath`  

The index path of the data item that the cell represented.

## Discussion

Use this method to detect when a cell is removed from a collection view, as opposed to monitoring the view itself to see when it disappears.

## See Also

### Tracking the addition and removal of views

func collectionView(UICollectionView, willDisplay: UICollectionViewCell, forItemAt: IndexPath)

Tells the delegate that the specified cell is about to be displayed in the collection view.

func collectionView(UICollectionView, willDisplaySupplementaryView: UICollectionReusableView, forElementKind: String, at: IndexPath)

Tells the delegate that the specified supplementary view is about to be displayed in the collection view.

func collectionView(UICollectionView, didEndDisplayingSupplementaryView: UICollectionReusableView, forElementOfKind: String, at: IndexPath)

Tells the delegate that the specified supplementary view was removed from the collection view.

