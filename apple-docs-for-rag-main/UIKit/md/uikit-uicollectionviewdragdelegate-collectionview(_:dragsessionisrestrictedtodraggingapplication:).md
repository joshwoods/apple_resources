

- UIKit
- UICollectionViewDragDelegate
-  collectionView(\_:dragSessionIsRestrictedToDraggingApplication:) 

Instance Method

# collectionView(\_:dragSessionIsRestrictedToDraggingApplication:)

Returns a Boolean value that determines whether the source app and destination app must be the same for a drag session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    dragSessionIsRestrictedToDraggingApplication session: any UIDragSession
) -> Bool
```

## Parameters 

`collectionView`  

The collection view from which the drag operation originated.

`session`  

The drag session that’s active.

## Return Value

true when the source app and destination app should be the same — that is, the user is not allowed to drop the item on another app.

## Discussion

If you don’t implement this method, the default return value is false.

## See Also

### Controlling the drag session

func collectionView(UICollectionView, dragSessionAllowsMoveOperation: any UIDragSession) -> Bool

Returns a Boolean value that determines whether a move operation is allowed for a drag session.

