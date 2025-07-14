

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:canDragItemsAt:with:) 

Instance Method

# collectionView(\_:canDragItemsAt:with:)

Returns a Boolean indicating whether a drag operation involving the specified items can begin.

macOS 10.11+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    canDragItemsAt indexPaths: Set,
    with event: NSEvent
) -> Bool
```

## Parameters 

`collectionView`  

The collection view making the request.

`indexPaths`  

The index paths of the items about to be dragged.

`event`  

The mouse-down event that began the drag operation.

## Return Value

true if the drag operation can begin or false if it cannot.

## Discussion

If you do not implement this method and your collection view has only one section, the collection view calls the legacy collectionView(_:canDragItemsAt:with:) method. If you do not implement either method, the collection view assumes a return value of true.

## See Also

### Drag and Drop Support

Supporting Collection View Drag and Drop Through File Promises

Share data between macOS apps during drag and drop by using an item provider.

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

func collectionView(NSCollectionView, acceptDrop: any NSDraggingInfo, indexPath: IndexPath, dropOperation: NSCollectionView.DropOperation) -> Bool

Incorporates the dropped content into the collection view.

