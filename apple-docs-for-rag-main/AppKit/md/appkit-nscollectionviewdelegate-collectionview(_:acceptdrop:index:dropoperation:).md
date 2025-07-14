

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:acceptDrop:index:dropOperation:) 

Instance Method

# collectionView(\_:acceptDrop:index:dropOperation:)

Invoked when the mouse is released over a collection view that previously allowed a drop.

macOS 10.6+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    acceptDrop draggingInfo: any NSDraggingInfo,
    index: Int,
    dropOperation: NSCollectionView.DropOperation
) -> Bool
```

## Parameters 

`collectionView`  

The collection view that send the message.

`draggingInfo`  

An object that contains more information about this dragging operation.

`index`  

The index of the proposed drop item.

`dropOperation`  

The type of dragging operation.

## Return Value

true if the drop operation should be accepted, otherwise false.

## Discussion

This method is called when the mouse is released over a collection view that previously decided to allow a drop via the collectionView(_:validateDrop:proposedIndex:dropOperation:) method. At this time, the delegate should incorporate the data from the dragging pasteboard and update the collection view’s contents.

You must implement this method for your collection view to be a drag destination

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

func collectionView(NSCollectionView, draggingSession: NSDraggingSession, willBeginAt: NSPoint, forItemsAt: IndexSet)

Notifies your delegate that a drag session is about to begin.

func collectionView(NSCollectionView, validateDrop: any NSDraggingInfo, proposedIndex: UnsafeMutablePointer&lt;Int>, dropOperation: UnsafeMutablePointer&lt;NSCollectionView.DropOperation>) -> NSDragOperation

Validates the specified location to see if it is a valid drop target.

