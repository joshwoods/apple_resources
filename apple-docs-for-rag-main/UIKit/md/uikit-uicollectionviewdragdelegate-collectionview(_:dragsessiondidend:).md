

- UIKit
- UICollectionViewDragDelegate
-  collectionView(\_:dragSessionDidEnd:) 

Instance Method

# collectionView(\_:dragSessionDidEnd:)

Notifies you that a drag session ended for the collection view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    dragSessionDidEnd session: any UIDragSession
)
```

## Parameters 

`collectionView`  

The collection view from which the drag operation originated.

`session`  

The drag session that ended.

## Discussion

This method is called after the drag session ended, usually because the content was dropped but possibly because the drag was terminated. Use this method to close out any tasks related to the management of the drag session in your app.

Each call to this method is always balanced by a call to the collectionView(_:dragSessionWillBegin:) method.

## See Also

### Tracking the drag session

func collectionView(UICollectionView, dragSessionWillBegin: any UIDragSession)

Notifies you that a drag session is about to begin for the collection view.

