

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:namesOfPromisedFilesDroppedAtDestination:forDraggedItemsAt:) Deprecated

Instance Method

# collectionView(\_:namesOfPromisedFilesDroppedAtDestination:forDraggedItemsAt:)

Invoked to return an array of filenames that the receiver promises to create.

macOS 10.6–10.13Deprecated

``` source
optional func collectionView(
    _ collectionView: NSCollectionView,
    namesOfPromisedFilesDroppedAtDestination dropURL: URL,
    forDraggedItemsAt indexes: IndexSet
) -> [String]
```

Deprecated

Use NSFilePromiseReceiver objects instead

## Parameters 

`collectionView`  

The collection view that send the message.

`dropURL`  

The drop location where the files are created.

`indexes`  

The indexes of the dragging items.

## Return Value

An array of filenames (not full paths) for the created files that the receiver promises to create.

## Discussion

The delegate can support file promise drags by adding NSFilesPromisePboardType to the pasteboard in collectionView(_:writeItemsAt:to:).

For more information on file promise dragging, see documentation for the NSDraggingSource protocol and namesOfPromisedFilesDropped(atDestination:).

You do not need to implement this delegate method for your collection view to be a drag source.

## See Also

### Legacy Collection View Support

func collectionView(NSCollectionView, canDragItemsAt: IndexSet, with: NSEvent) -> Bool

Returns a Boolean indicating whether the collection view can begin dragging the specified items.

func collectionView(NSCollectionView, pasteboardWriterForItemAt: Int) -> (any NSPasteboardWriting)?

Provides the pasteboard writer for the item at the specified index

func collectionView(NSCollectionView, writeItemsAt: IndexSet, to: NSPasteboard) -> Bool

Invoked after it has been determined that a drag should begin, but before the drag has been started.

Deprecated

func collectionView(NSCollectionView, draggingImageForItemsAt: IndexSet, with: NSEvent, offset: NSPointPointer) -> NSImage

Creates and returns a drag image to represent the specified items during a drag.

func collectionView(NSCollectionView, draggingSession: NSDraggingSession, willBeginAt: NSPoint, forItemsAt: IndexSet)

Notifies your delegate that a drag session is about to begin.

func collectionView(NSCollectionView, validateDrop: any NSDraggingInfo, proposedIndex: UnsafeMutablePointer&lt;Int>, dropOperation: UnsafeMutablePointer&lt;NSCollectionView.DropOperation>) -> NSDragOperation

Validates the specified location to see if it is a valid drop target.

func collectionView(NSCollectionView, acceptDrop: any NSDraggingInfo, index: Int, dropOperation: NSCollectionView.DropOperation) -> Bool

Invoked when the mouse is released over a collection view that previously allowed a drop.

