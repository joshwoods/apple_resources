

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:draggingSession:willBeginAt:forItemsAt:) 

Instance Method

# collectionView(\_:draggingSession:willBeginAt:forItemsAt:)

Notifies your delegate that a drag session is about to begin.

macOS 10.10+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    draggingSession session: NSDraggingSession,
    willBeginAt screenPoint: NSPoint,
    forItemsAt indexes: IndexSet
)
```

## Parameters 

`collectionView`  

The collection view notifying your delegate object.

`session`  

The dragging session that is about to begin.

`screenPoint`  

The starting point (in screen coordinates) for the drag operation.

`indexes`  

The indexes of the items being dragged.

## Discussion

You can use this method to modify the dragging session or to perform other tasks related to the beginning of a drag session.

## See Also

### Legacy Collection View Support

func collectionView(NSCollectionView, canDragItemsAt: IndexSet, with: NSEvent) -> Bool

Returns a Boolean indicating whether the collection view can begin dragging the specified items.

func collectionView(NSCollectionView, pasteboardWriterForItemAt: Int) -> (any NSPasteboardWriting)?

Provides the pasteboard writer for the item at the specified index

func collectionView(NSCollectionView, writeItemsAt: IndexSet, to: NSPasteboard) -> Bool

Invoked after it has been determined that a drag should begin, but before the drag has been started.

Deprecated

func collectionView(NSCollectionView, namesOfPromisedFilesDroppedAtDestination: URL, forDraggedItemsAt: IndexSet) -> [String]

Invoked to return an array of filenames that the receiver promises to create.

Deprecated

func collectionView(NSCollectionView, draggingImageForItemsAt: IndexSet, with: NSEvent, offset: NSPointPointer) -> NSImage

Creates and returns a drag image to represent the specified items during a drag.

func collectionView(NSCollectionView, validateDrop: any NSDraggingInfo, proposedIndex: UnsafeMutablePointer&lt;Int>, dropOperation: UnsafeMutablePointer&lt;NSCollectionView.DropOperation>) -> NSDragOperation

Validates the specified location to see if it is a valid drop target.

func collectionView(NSCollectionView, acceptDrop: any NSDraggingInfo, index: Int, dropOperation: NSCollectionView.DropOperation) -> Bool

Invoked when the mouse is released over a collection view that previously allowed a drop.

