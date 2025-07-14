

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:willDisplay:forItemAt:) 

Instance Method

# collectionView(\_:willDisplay:forItemAt:)

Tells the delegate that the specified cell is about to be displayed in the collection view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    willDisplay cell: UICollectionViewCell,
    forItemAt indexPath: IndexPath
)
```

## Parameters 

`collectionView`  

The collection view object that is adding the cell.

`cell`  

The cell object being added.

`indexPath`  

The index path of the data item that the cell represents.

## Discussion

The collection view calls this method before adding a cell to its content. Use this method to detect cell additions, as opposed to monitoring the cell itself to see when it appears.

## See Also

### Tracking the addition and removal of views

func collectionView(UICollectionView, willDisplaySupplementaryView: UICollectionReusableView, forElementKind: String, at: IndexPath)

Tells the delegate that the specified supplementary view is about to be displayed in the collection view.

func collectionView(UICollectionView, didEndDisplaying: UICollectionViewCell, forItemAt: IndexPath)

Tells the delegate that the specified cell was removed from the collection view.

func collectionView(UICollectionView, didEndDisplayingSupplementaryView: UICollectionReusableView, forElementOfKind: String, at: IndexPath)

Tells the delegate that the specified supplementary view was removed from the collection view.

