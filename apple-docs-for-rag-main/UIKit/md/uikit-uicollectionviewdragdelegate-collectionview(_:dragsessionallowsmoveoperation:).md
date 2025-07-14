

- UIKit
- UICollectionViewDragDelegate
-  collectionView(\_:dragSessionAllowsMoveOperation:) 

Instance Method

# collectionView(\_:dragSessionAllowsMoveOperation:)

Returns a Boolean value that determines whether a move operation is allowed for a drag session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    dragSessionAllowsMoveOperation session: any UIDragSession
) -> Bool
```

## Parameters 

`collectionView`  

The collection view from which the drag operation originated.

`session`  

The drag session that’s active.

## Return Value

false to cancel the drag session if move is not allowed; otherwise, true.

## Discussion

If you don’t implement this method, the default return value is true.

## See Also

### Controlling the drag session

func collectionView(UICollectionView, dragSessionIsRestrictedToDraggingApplication: any UIDragSession) -> Bool

Returns a Boolean value that determines whether the source app and destination app must be the same for a drag session.

