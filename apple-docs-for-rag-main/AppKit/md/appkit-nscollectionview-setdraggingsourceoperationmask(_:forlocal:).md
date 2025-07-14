

- AppKit
- NSCollectionView
-  setDraggingSourceOperationMask(\_:forLocal:) 

Instance Method

# setDraggingSourceOperationMask(\_:forLocal:)

Configures the default value returned from draggingSourceOperationMaskForLocal:.

macOS 10.6+

``` source
@MainActor
func setDraggingSourceOperationMask(
    _ dragOperationMask: NSDragOperation,
    forLocal localDestination: Bool
)
```

## Parameters 

`dragOperationMask`  

The types of drag operations allowed.

`localDestination`  

If true, mask applies when the drag destination object is in the same application as the receiver; if false, mask applies when the destination object is outside the receiver’s application.

## Discussion

By default, this method returns every when `localDestination` is true and NSDragOperationNone when `localDestination` is false. `NSCollectionView` will save the values you set for each `localDestination` value.

You typically will invoke this method, and not override it.

## See Also

### Legacy Collection View Support

var itemPrototype: NSCollectionViewItem?

The receiver’s collection view item prototype.

Deprecated

func newItem(forRepresentedObject: Any) -> NSCollectionViewItem

Returns the collection view item that is used for the specified object.

Deprecated

var selectionIndexes: IndexSet

The indexes of the currently selected items.

var maxNumberOfRows: Int

The maximum number of rows that the collection view displays.

Deprecated

var maxNumberOfColumns: Int

The maximum number of columns that the collection view displays.

Deprecated

var minItemSize: NSSize

The minimum size (in points) of items in the collection view grid.

Deprecated

var maxItemSize: NSSize

The maximum size (in points) of items in the collection view grid.

Deprecated

func item(at: Int) -> NSCollectionViewItem?

Returns the collection view item for the represented object at the specified index.

func frameForItem(at: Int) -> NSRect

Returns the frame of the collection view item at the specified index.

func frameForItem(at: Int, withNumberOfItems: Int) -> NSRect

Returns the frame of an item based on the number of items in the collection view.

func draggingImageForItems(at: IndexSet, with: NSEvent, offset: NSPointPointer) -> NSImage

This method computes and returns an image to use for dragging.

