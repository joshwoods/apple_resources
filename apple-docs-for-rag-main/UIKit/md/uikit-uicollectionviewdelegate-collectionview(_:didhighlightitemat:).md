

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:didHighlightItemAt:) 

Instance Method

# collectionView(\_:didHighlightItemAt:)

Tells the delegate that the item at the specified index path was highlighted.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    didHighlightItemAt indexPath: IndexPath
)
```

## Parameters 

`collectionView`  

The collection view object that is notifying you of the highlight change.

`indexPath`  

The index path of the cell that was highlighted.

## Discussion

The collection view calls this method only in response to user interactions and does not call it if you programmatically set the highlighting on a cell.

## See Also

### Managing cell highlighting

func collectionView(UICollectionView, shouldHighlightItemAt: IndexPath) -> Bool

Asks the delegate if the item should be highlighted during tracking.

func collectionView(UICollectionView, didUnhighlightItemAt: IndexPath)

Tells the delegate that the highlight was removed from the item at the specified index path.

