

- UIKit
- UICollectionViewDropDelegate
-  collectionView(\_:dropSessionDidExit:) 

Instance Method

# collectionView(\_:dropSessionDidExit:)

Notifies you when dragged content exits the collection view’s bounds rectangle.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    dropSessionDidExit session: any UIDropSession
)
```

## Parameters 

`collectionView`  

The collection view that was tracking the dragged content.

`session`  

The drop session object containing information about the type of data being dragged.

## Discussion

UIKit calls this method when dragged content exits the bounds rectangle of the specified collection view. The method isn’t called again until the dragged content enters the collection view’s bounds (triggering a call to the collectionView(_:dropSessionDidEnter:) method) and exits again.

Use this method to clean up any state information that you configured in your collectionView(_:dropSessionDidEnter:) method.

## See Also

### Tracking the drag movements

func collectionView(UICollectionView, dropSessionDidUpdate: any UIDropSession, withDestinationIndexPath: IndexPath?) -> UICollectionViewDropProposal

Tells your delegate that the position of the dragged data over the collection view changed.

func collectionView(UICollectionView, dropSessionDidEnter: any UIDropSession)

Notifies you when dragged content enters the collection view’s bounds rectangle.

func collectionView(UICollectionView, dropSessionDidEnd: any UIDropSession)

Notifies you when the drag operation ends.

