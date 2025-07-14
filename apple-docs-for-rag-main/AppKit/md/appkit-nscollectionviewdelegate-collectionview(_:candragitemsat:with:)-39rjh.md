

- AppKit
- NSCollectionViewDelegate
-  collectionView(\_:canDragItemsAt:with:) 

Instance Method

# collectionView(\_:canDragItemsAt:with:)

Returns a Boolean indicating whether the collection view can begin dragging the specified items.

macOS 10.6+

``` source
@MainActor
optional func collectionView(
    _ collectionView: NSCollectionView,
    canDragItemsAt indexes: IndexSet,
    with event: NSEvent
) -> Bool
```

## Parameters 

`collectionView`  

The collection view containing the items to be dragged.

`indexes`  

The indexes of the items to be dragged.

`event`  

The mouse event that initiated the drag action.

## Return Value

true if the collection view can begin the drag operation for the specified items or false if it cannot.

## Discussion

Implement this method when you want selective control over the initiation of drag operations. In your implementation, use the provided information to determine whether the drag operation should occur and return the appropriate return value. For example, you might return false if your interface does not allow the user to drag the specified items.

If you do not implement this method in your delegate object, the collection view assumes a return value of true and begins the drag operation.

## See Also

### Legacy Collection View Support

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

func collectionView(NSCollectionView, acceptDrop: any NSDraggingInfo, index: Int, dropOperation: NSCollectionView.DropOperation) -> Bool

Invoked when the mouse is released over a collection view that previously allowed a drop.

