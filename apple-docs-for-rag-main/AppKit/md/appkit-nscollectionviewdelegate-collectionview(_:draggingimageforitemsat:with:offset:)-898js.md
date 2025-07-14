

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:draggingImageForItemsAt:with:offset:) 

Instance Method

# collectionView(\_:draggingImageForItemsAt:with:offset:)

Creates and returns a drag image to represent the specified items during a drag.

macOS 10.11+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    draggingImageForItemsAt indexPaths: Set,
    with event: NSEvent,
    offset dragImageOffset: NSPointPointer
) -> NSImage
```

## Parameters 

`collectionView`  

The collection view making the request.

`indexPaths`  

The index paths of the items being dragged.

`event`  

The mouse-down event that began the drag operation. You can use the mouse location when determining what value to return in the `dragImageOffset` parameter.

`dragImageOffset`  

The offset value to use when positioning the image. On input, the point is NSZeroPoint, which centers the returned image under the mouse. Your method can return a different point that repositions the drag image by the specified offset values.

## Return Value

The image to use for the dragged items.

## Discussion

Your implementation of this method should create an appropriate image to use during the drag operation. The collection view places the center of your image at the current mouse location. Update the value in the `dragImageOffset` parameter to shift the position of your image by the specified amount.

If you do not implement this method, the collection view uses the drag image returned by the draggingImageForItems(at:with:offset:) method instead.

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

