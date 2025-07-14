

- UIKit
- UICollectionViewDelegate
-  collectionView(\_:shouldHighlightItemAt:) 

Instance Method

# collectionView(\_:shouldHighlightItemAt:)

Asks the delegate if the item should be highlighted during tracking.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    shouldHighlightItemAt indexPath: IndexPath
) -> Bool
```

## Parameters 

`collectionView`  

The collection view object that is asking about the highlight change.

`indexPath`  

The index path of the cell to be highlighted.

## Return Value

true if the item should be highlighted or false if it should not.

## Discussion

As touch events arrive, the collection view highlights items in anticipation of the user selecting them. As it processes those touch events, the collection view calls this method to ask your delegate if a given cell should be highlighted. It calls this method only in response to user interactions and does not call it if you programmatically set the highlighting on a cell.

If you return false in your implementation, the cell does not get highlighted and the system bypasses the entire selection process. That is, the system does not call collectionView(_:shouldSelectItemAt:) or any other selection-related methods. If you return true, isHighlighted is set to true, collectionView(_:didHighlightItemAt:) is called, and the system begins the selection process.

If you do not implement this method, the default return value is true.

## See Also

### Managing cell highlighting

func collectionView(UICollectionView, didHighlightItemAt: IndexPath)

Tells the delegate that the item at the specified index path was highlighted.

func collectionView(UICollectionView, didUnhighlightItemAt: IndexPath)

Tells the delegate that the highlight was removed from the item at the specified index path.

