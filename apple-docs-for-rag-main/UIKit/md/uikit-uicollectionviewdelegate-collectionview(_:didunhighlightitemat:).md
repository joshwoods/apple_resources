

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:didUnhighlightItemAt:) 

Instance Method

# collectionView(\_:didUnhighlightItemAt:)

Tells the delegate that the highlight was removed from the item at the specified index path.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    didUnhighlightItemAt indexPath: IndexPath
)
```

## Parameters 

`collectionView`  

The collection view object that is notifying you of the highlight change.

`indexPath`  

The index path of the cell that had its highlight removed.

## Discussion

The collection view calls this method only in response to user interactions and does not call it if you programmatically change the highlighting on a cell.

## See Also

### Managing cell highlighting

func collectionView(UICollectionView, shouldHighlightItemAt: IndexPath) -> Bool

Asks the delegate if the item should be highlighted during tracking.

func collectionView(UICollectionView, didHighlightItemAt: IndexPath)

Tells the delegate that the item at the specified index path was highlighted.

