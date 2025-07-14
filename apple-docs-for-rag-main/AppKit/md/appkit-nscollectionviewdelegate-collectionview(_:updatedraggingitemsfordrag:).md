

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:updateDraggingItemsForDrag:) 

Instance Method

# collectionView(\_:updateDraggingItemsForDrag:)

Asks your delegate to update the dragging items during a drag operation.

macOS 10.5+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    updateDraggingItemsForDrag draggingInfo: any NSDraggingInfo
)
```

## Parameters 

`collectionView`  

The collection view asking you to update the dragging items.

`draggingInfo`  

The current information for the drag operation. Use this object to iterate over the dragging items.

## Discussion

You can use this method to update the current drag items while a drag is in progress. Updating the drag items is optional, but you might use this method to change the image for an item. For example, you might change the image when the mouse hovers over a particular part of the collection view. Use the enumerateDraggingItems(options:for:classes:searchOptions:using:) method of the `draggingInfo` parameter to iterate over the drag items and update them as appropriate.

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

func collectionView(NSCollectionView, validateDrop: any NSDraggingInfo, proposedIndexPath: AutoreleasingUnsafeMutablePointer&lt;NSIndexPath>, dropOperation: UnsafeMutablePointer&lt;NSCollectionView.DropOperation>) -> NSDragOperation

Validates whether a drop operation is possible at the specified location.

func collectionView(NSCollectionView, acceptDrop: any NSDraggingInfo, indexPath: IndexPath, dropOperation: NSCollectionView.DropOperation) -> Bool

Incorporates the dropped content into the collection view.

