

- UIKit
- UICollectionViewDragDelegate
-  collectionView(\_:dragSessionWillBegin:) 

Instance Method

# collectionView(\_:dragSessionWillBegin:)

Notifies you that a drag session is about to begin for the collection view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    dragSessionWillBegin session: any UIDragSession
)
```

## Parameters 

`collectionView`  

The collection view from which the drag operation originated.

`session`  

The drag session that’s beginning.

## Discussion

This method is called after it has been determined that a drag will begin and after any lift animations have occurred, but before the position of the drag changes. Use this method to perform any tasks related to the management of the drag session in your app.

Each call to this method is always balanced by a call to the collectionView(_:dragSessionDidEnd:) method.

## See Also

### Tracking the drag session

func collectionView(UICollectionView, dragSessionDidEnd: any UIDragSession)

Notifies you that a drag session ended for the collection view.

