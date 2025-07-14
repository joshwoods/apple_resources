

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:writeItemsAt:to:) Deprecated

Instance Method

# collectionView(\_:writeItemsAt:to:)

Invoked after it has been determined that a drag should begin, but before the drag has been started.

macOS 10.6–10.15Deprecated

``` source
optional func collectionView(
    _ collectionView: NSCollectionView,
    writeItemsAt indexes: IndexSet,
    to pasteboard: NSPasteboard
) -> Bool
```

Deprecated

Use -collectionView:pasteboardWriterForItemAtIndexPath: instead

## Parameters 

`collectionView`  

The collection view that send the message.

`indexes`  

The indexes of the items to write to the pasteboard.

`pasteboard`  

The pasteboard containing the content from the dragged items.

## Return Value

true to begin the drag, otherwise false.

## Discussion

To start the drag, you must first declare the pasteboard types that are supported by sending `pasteboard` a declareTypes(_:owner:) method. You then place the data for the items at the specified indexes on `pasteboard`, and return true from the method.

The drag image and other drag related information will be set up and provided by the view once this call returns true.

You need to implement this method for your collection view to be a drag source.

## See Also

### Legacy Collection View Support

func collectionView(NSCollectionView, canDragItemsAt: IndexSet, with: NSEvent) -> Bool

Returns a Boolean indicating whether the collection view can begin dragging the specified items.

func collectionView(NSCollectionView, pasteboardWriterForItemAt: Int) -> (any NSPasteboardWriting)?

Provides the pasteboard writer for the item at the specified index

func collectionView(NSCollectionView, namesOfPromisedFilesDroppedAtDestination: URL, forDraggedItemsAt: IndexSet) -> [String]

Invoked to return an array of filenames that the receiver promises to create.

Deprecated

func collectionView(NSCollectionView, draggingImageForItemsAt: IndexSet, with: NSEvent, offset: NSPointPointer) -> NSImage

Creates and returns a drag image to represent the specified items during a drag.

func collectionView(NSCollectionView, draggingSession: NSDraggingSession, willBeginAt: NSPoint, forItemsAt: IndexSet)

Notifies your delegate that a drag session is about to begin.

func collectionView(NSCollectionView, validateDrop: any NSDraggingInfo, proposedIndex: UnsafeMutablePointer&lt;Int>, dropOperation: UnsafeMutablePointer&lt;NSCollectionView.DropOperation>) -> NSDragOperation

Validates the specified location to see if it is a valid drop target.

func collectionView(NSCollectionView, acceptDrop: any NSDraggingInfo, index: Int, dropOperation: NSCollectionView.DropOperation) -> Bool

Invoked when the mouse is released over a collection view that previously allowed a drop.

