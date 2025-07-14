

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:pasteboardWriterForItemAt:) 

Instance Method

# collectionView(\_:pasteboardWriterForItemAt:)

Provides the pasteboard writer for the item at the specified index

macOS 10.5+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    pasteboardWriterForItemAt index: Int
) -> (any NSPasteboardWriting)?
```

## Parameters 

`collectionView`  

The collection view making the request.

`index`  

The index of the item requiring a pasteboard writer.

## Return Value

The pasteboard writer object to use for managing the item data. Return `nil` to prevent the collection view from dragging the item.

## Discussion

The collection view calls this method for each item involved in the drag operation after it has determined that a drag should begin but before the drag operation has started. Your implementation of this method should create and return the pasteboard writer—an object conforming to the NSPasteboardWriting protocol—to use for providing the item’s data. Using the object you provide, the collection view creates an NSDraggingItem object for you and configures its draggingFrame and imageComponents properties for you using information from the item at the specified index path.

If you implement this method, the collection view does not call the collectionView(_:draggingImageForItemsAt:with:offset:) of your delegate or the draggingImageForItems(at:with:offset:) method of NSCollectionView.

## See Also

### Legacy Collection View Support

func collectionView(NSCollectionView, canDragItemsAt: IndexSet, with: NSEvent) -> Bool

Returns a Boolean indicating whether the collection view can begin dragging the specified items.

func collectionView(NSCollectionView, writeItemsAt: IndexSet, to: NSPasteboard) -> Bool

Invoked after it has been determined that a drag should begin, but before the drag has been started.

Deprecated

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

