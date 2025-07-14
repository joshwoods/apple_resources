

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:namesOfPromisedFilesDroppedAtDestination:forDraggedItemsAt:) Deprecated

Instance Method

# collectionView(\_:namesOfPromisedFilesDroppedAtDestination:forDraggedItemsAt:)

Returns the names of the promised files that you created for a drag operation.

macOS 10.11–10.13Deprecated

``` source
optional func collectionView(
    _ collectionView: NSCollectionView,
    namesOfPromisedFilesDroppedAtDestination dropURL: URL,
    forDraggedItemsAt indexPaths: Set
) -> [String]
```

Deprecated

Use NSFilePromiseReceiver objects instead

## Parameters 

`collectionView`  

The collection view asking you to provide the list of filenames.

`dropURL`  

The URL at which to create the promised files.

`indexPaths`  

The index paths of the dragged items.

## Return Value

An array of strings containing the filenames you created, or intend to create, at the specified URL.

## Discussion

At the start of a drag operation, your app must provide the data that constitutes the items being dragged. If you specify a file promise, instead of the data itself, use this method to specify the names of the files you promised. If the files already exist, move them to the directory specified by the `dropURL` parameter. If you must create the files first, use this method to specify the names of the files you intend to provide and begin creating those files asynchronously on a background thread.

The filenames you return are made available from the namesOfPromisedFilesDropped(atDestination:) method of the NSDraggingInfo object passed around during the drag operation.

For more information about how to use file promises when dragging content, see Drag and Drop Programming Topics.

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

