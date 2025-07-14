

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:pasteboardWriterForItemAt:) 

Instance Method

# collectionView(\_:pasteboardWriterForItemAt:)

Provides the pasteboard writer for the item at the specified index path.

macOS 10.11+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    pasteboardWriterForItemAt indexPath: IndexPath
) -> (any NSPasteboardWriting)?
```

## Parameters 

`collectionView`  

The collection view making the request.

`indexPath`  

The index path of the item requiring a pasteboard writer.

## Return Value

The pasteboard writer object to use for managing the item data. Return `nil` to prevent the collection view from dragging the item.

## Discussion

You must implement this method or the collectionView(_:writeItemsAt:to:) method to support drag operations. The collection view calls this method in preference over the collectionView(_:writeItemsAt:to:) method if both are implemented. If your app supports multi-image drag and drop, you must implement this method.

The collection view calls this method for each item involved in the drag operation after it has determined that a drag should begin but before the drag operation has started. Your implementation of this method should create and return the pasteboard writer—an object conforming to the NSPasteboardWriting protocol—to use for providing the item’s data. Using the object you provide, the collection view creates an NSDraggingItem object for you and configures its draggingFrame and imageComponents properties for you using information from the item at the specified index path.

If you implement this method, the collection view does not call the collectionView(_:draggingImageForItemsAt:with:offset:) of your delegate or the draggingImageForItems(at:with:offset:) method of NSCollectionView.

## See Also

### Drag and Drop Support

Supporting Collection View Drag and Drop Through File Promises

Share data between macOS apps during drag and drop by using an item provider.

func collectionView(NSCollectionView, canDragItemsAt: Set&lt;IndexPath>, with: NSEvent) -> Bool

Returns a Boolean indicating whether a drag operation involving the specified items can begin.

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

func collectionView(NSCollectionView, acceptDrop: any NSDraggingInfo, indexPath: IndexPath, dropOperation: NSCollectionView.DropOperation) -> Bool

Incorporates the dropped content into the collection view.

