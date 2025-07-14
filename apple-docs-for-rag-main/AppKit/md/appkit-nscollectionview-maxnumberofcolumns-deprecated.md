

- AppKit
- NSCollectionView
-  maxNumberOfColumns Deprecated

Instance Property

# maxNumberOfColumns

The maximum number of columns that the collection view displays.

macOS 10.5–10.14Deprecated

``` source
@MainActor
var maxNumberOfColumns: Int { get set }
```

Deprecated

Use NSCollectionViewGridLayout as the receiver's collectionViewLayout, setting its maximumNumberOfColumns instead

## Discussion

When the value of this property is `0`, the collection view has no maximum number of columns. The default value of this property is `0`.

It is possible for a collection view to specify both a maximum number of rows and a maximum number of columns. If the number of content objects exceeds the number of displayable items (*n*=`maxNumberOfRows` \* `maxNumberOfColumns`) only the first *n* items of the content array are displayed.

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

func setDraggingSourceOperationMask(NSDragOperation, forLocal: Bool)

Configures the default value returned from draggingSourceOperationMaskForLocal:.

