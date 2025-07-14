

- UIKit
- UICollectionViewDropDelegate
-  collectionView(\_:dropSessionDidUpdate:withDestinationIndexPath:) 

Instance Method

# collectionView(\_:dropSessionDidUpdate:withDestinationIndexPath:)

Tells your delegate that the position of the dragged data over the collection view changed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func collectionView(
    _ collectionView: UICollectionView,
    dropSessionDidUpdate session: any UIDropSession,
    withDestinationIndexPath destinationIndexPath: IndexPath?
) -> UICollectionViewDropProposal
```

## Parameters 

`collectionView`  

The collection view that’s tracking the dragged content.

`session`  

The drop session object containing information about the type of data being dragged.

`destinationIndexPath`  

The index path at which the content would be dropped.

## Return Value

Your proposal for how to handle the content if it is dropped at the specified location.

## Mentioned in 

Supporting Drag and Drop in Collection Views

## Discussion

While the user is dragging content, the collection view calls this method repeatedly to determine how you would handle the drop if it occurred at the specified location. The collection view provides visual feedback to the user based on your proposal.

In your implementation of this method, create a UICollectionViewDropProposal object and use it to convey your intentions. Because this method is called repeatedly while the user drags over the table view, your implementation should return as quickly as possible.

## See Also

### Tracking the drag movements

func collectionView(UICollectionView, dropSessionDidEnter: any UIDropSession)

Notifies you when dragged content enters the collection view’s bounds rectangle.

func collectionView(UICollectionView, dropSessionDidExit: any UIDropSession)

Notifies you when dragged content exits the collection view’s bounds rectangle.

func collectionView(UICollectionView, dropSessionDidEnd: any UIDropSession)

Notifies you when the drag operation ends.

