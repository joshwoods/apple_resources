

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:writeItemsAt:to:) Deprecated

Instance Method

# collectionView(\_:writeItemsAt:to:)

Places the data for the drag operation on the pasteboard.

macOS 10.11–10.15Deprecated

``` source
optional func collectionView(
    _ collectionView: NSCollectionView,
    writeItemsAt indexPaths: Set,
    to pasteboard: NSPasteboard
) -> Bool
```

Deprecated

Use -collectionView:pasteboardWriterForItemAtIndexPath: instead

## Parameters 

`collectionView`  

The collection view making the request.

`indexPaths`  

The index paths of the items being dragged.

`pasteboard`  

The pasteboard on which to place the drag data.

## Return Value

true if the drag operation can continue or false if you want to refuse the drag.

## Discussion

You must implement this method or the collectionView(_:pasteboardWriterForItemAt:) method to support drag operations. The collection view calls the collectionView(_:pasteboardWriterForItemAt:) method in preference to this one if both are implemented. If your app supports multi-image drag and drop, you must implement the collectionView(_:pasteboardWriterForItemAt:) method.

The collection view calls this method after it has determined that a drag should begin but before the drag operation has started. Your implementation of this method should do the following:

1.  Declare the pasteboard types you support using the declareTypes(_:owner:) method of the provided `pasteboard` object.

2.  Write data to the pasteboard for each type you declare.

3.  Return true from this method.

## See Also

### Drag and Drop Support

Supporting Collection View Drag and Drop Through File Promises

Share data between macOS apps during drag and drop by using an item provider.

func collectionView(NSCollectionView, canDragItemsAt: Set&lt;IndexPath>, with: NSEvent) -> Bool

Returns a Boolean indicating whether a drag operation involving the specified items can begin.

func collectionView(NSCollectionView, pasteboardWriterForItemAt: IndexPath) -> (any NSPasteboardWriting)?

Provides the pasteboard writer for the item at the specified index path.

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

