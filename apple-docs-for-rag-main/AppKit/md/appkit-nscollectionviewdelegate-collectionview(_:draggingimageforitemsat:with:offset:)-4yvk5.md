

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:draggingImageForItemsAt:with:offset:) 

Instance Method

# collectionView(\_:draggingImageForItemsAt:with:offset:)

Creates and returns a drag image to represent the specified items during a drag.

macOS 10.6+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    draggingImageForItemsAt indexes: IndexSet,
    with event: NSEvent,
    offset dragImageOffset: NSPointPointer
) -> NSImage
```

## Parameters 

`collectionView`  

The collection view making the request.

`indexes`  

The indexes of the items being dragged.

`event`  

The mouse-down event that initiated the drag.

`dragImageOffset`  

An in/out parameter that is initially set to NSZeroPoint, which causes the image to be centered under the mouse. The value can be modified to reposition the returned image.

## Return Value

The image to use for the dragged items.

## Discussion

If the delegate does not implement this method, the collection view uses the image returned by draggingImageForItems(at:with:offset:).

You do not need to implement this method for your collection view to be a drag source.

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

func collectionView(NSCollectionView, draggingSession: NSDraggingSession, willBeginAt: NSPoint, forItemsAt: IndexSet)

Notifies your delegate that a drag session is about to begin.

func collectionView(NSCollectionView, validateDrop: any NSDraggingInfo, proposedIndex: UnsafeMutablePointer&lt;Int>, dropOperation: UnsafeMutablePointer&lt;NSCollectionView.DropOperation>) -> NSDragOperation

Validates the specified location to see if it is a valid drop target.

func collectionView(NSCollectionView, acceptDrop: any NSDraggingInfo, index: Int, dropOperation: NSCollectionView.DropOperation) -> Bool

Invoked when the mouse is released over a collection view that previously allowed a drop.

