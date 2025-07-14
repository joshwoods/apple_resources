

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:acceptDrop:indexPath:dropOperation:) 

Instance Method

# collectionView(\_:acceptDrop:indexPath:dropOperation:)

Incorporates the dropped content into the collection view.

macOS 10.11+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    acceptDrop draggingInfo: any NSDraggingInfo,
    indexPath: IndexPath,
    dropOperation: NSCollectionView.DropOperation
) -> Bool
```

## Parameters 

`collectionView`  

The collection view receiving the dropped content.

`draggingInfo`  

The information about the drag operation.

`indexPath`  

The index path at which the drop occurred. Use this location as the insertion point for the content.

`dropOperation`  

The type of drop operation to perform.

## Return Value

true if the drop operation should be accepted or false if it should be rejected.

## Discussion

The collection view calls this method when the user releases the mouse button while it is over a valid drop target. This method is called after the collectionView(_:validateDrop:proposedIndexPath:dropOperation:) method validates that dropping the content at the specified location is possible. You must implement this method to accept the dropped content and incorporate it into the collection view.

In your implementation, use the information in the `draggingInfo` parameter to retrieve the data, update your data source object, and insert the appropriate items into the collection view. The dropped data is stored in the draggingPasteboard property of the dragging information object.

If the animatesToDestination property of the dragging information is true, update the image and frame for each dragged item to its new location in the collection view. You can enumerate the list of dragged items using the enumerateDraggingItems(options:for:classes:searchOptions:using:) method of the dragging information object.

## See Also

### Drag and Drop Support

Supporting Collection View Drag and Drop Through File Promises

Share data between macOS apps during drag and drop by using an item provider.

func collectionView(NSCollectionView, canDragItemsAt: Set&lt;IndexPath>, with: NSEvent) -> Bool

Returns a Boolean indicating whether a drag operation involving the specified items can begin.

func collectionView(NSCollectionView, pasteboardWriterForItemAt: IndexPath) -> (any NSPasteboardWriting)?

Provides the pasteboard writer for the item at the specified index path.

func collectionView(NSCollectionView, writeItemsAt: Set&lt;IndexPath>, to: NSPasteboard) -> Bool

Places the data for the drag operation on the pasteboard.

Deprecated

func collectionView(NSCollectionView, namesOfPromisedFilesDroppedAtDestination: URL, forDraggedItemsAt: Set&lt;IndexPath>) -> [String]

Returns the names of the promised files that you created for a drag operation.

Deprecated

func collectionView(NSCollectionView, draggingImageForItemsAt: Set&lt;IndexPath>, with: NSEvent, offset: NSPointPointer) -> NSImage

Creates and returns a drag image to represent the specified items during a drag.

func collectionView(NSCollectionView, draggingSession: NSDraggingSession, willBeginAt: NSPoint, forItemsAt: Set&lt;IndexPath>)

Notifies your delegate that a drag session is about to begin.

func collectionView(NSCollectionView, draggingSession: NSDraggingSession, endedAt: NSPoint, dragOperation: NSDragOperation)

Notifies your delegate that a drag session ended.

func collectionView(NSCollectionView, updateDraggingItemsForDrag: any NSDraggingInfo)

Asks your delegate to update the dragging items during a drag operation.

func collectionView(NSCollectionView, validateDrop: any NSDraggingInfo, proposedIndexPath: AutoreleasingUnsafeMutablePointer&lt;NSIndexPath>, dropOperation: UnsafeMutablePointer&lt;NSCollectionView.DropOperation>) -> NSDragOperation

Validates whether a drop operation is possible at the specified location.

