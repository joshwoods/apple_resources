

- Quartz
-  IKImageBrowserView Deprecated

Class

# IKImageBrowserView

A view for displaying and browsing a large collection of images and movies.

macOS 10.5–10.14Deprecated

``` source
@MainActor
class IKImageBrowserView
```

Deprecated

Deprecated - Please use NSCollectionView instead

## Overview

The IKImageBrowserView class is a view for displaying and browsing a large amount of images and movies efficiently. This class will be deprecated in a future release. Please switch to NSCollectionView instead.

You must set a datasource for the view and implement, at a minimum, the numberOfItems(inImageBrowser:) and imageBrowser(_:itemAt:) described in IKImageBrowserDataSource Protocol. The items must conform to the IKImageBrowserItem Protocol protocol.

The class’s delegate object must conform to IKImageBrowserDelegate Protocol protocol. It receives notification of changes in selection, as well as mouse events in the cells.

Core Animation Integration

The image browser supports either being hosted in a layer-backed view or using custom layers for its own appearance. Custom layers on the image browser are not supported when the image browser is itself backed by a layer.

## Topics

### Updating the Display of the Content

func reloadData()

Marks the receiver as needing its data reloaded.

### Getting and Setting the Delegate

var delegate: AnyObject!

Returns the delegate of the receiver.

### Getting and Setting the Data Source

var dataSource: AnyObject!

Returns the data source of the receiver.

### Setting the Appearance

func setCellsStyleMask(Int)

Defines the appearance style of the cells.

func cellsStyleMask() -> Int

Returns the appearance style mask for the cell.

func setConstrainsToOriginalSize(Bool)

Sets whether the receiver constrains the cell’s image to its original size.

func constrainsToOriginalSize() -> Bool

Returns whether the receiver constrains the cell’s image to its original size.

func setIntercellSpacing(NSSize)

Sets the spacing between cells in the view.

func intercellSpacing() -> NSSize

Returns the spacing between cells in the view.

### Creating a Custom Cell for an Item

func newCell(forRepresentedItem: Any!) -> IKImageBrowserCell!

Returns the cell to use for the specified item.

### Zooming and Resizing

func setZoomValue(Float)

Sets the zoom value.

func zoomValue() -> Float

Returns the current zoom value.

func setContentResizingMask(Int)

Determines how the receiver resizes its content when zooming.

func contentResizingMask() -> Int

Returns the receiver’s content resizing mask, which determines how its content is resized while zooming.

### Scrolling

func scrollIndexToVisible(Int)

Scrolls the receiver to the item at the specified index.

### Setting and Getting Cell Size

func setCellSize(NSSize)

Sets the cell size.

func cellSize() -> NSSize

Returns the cell size.

### Getting Item Information

func indexOfItem(at: NSPoint) -> Int

Returns the index of the item at the specified location.

func itemFrame(at: Int) -> NSRect

Returns the frame rectangle for the item located at the specified index.

func visibleItemIndexes() -> IndexSet!

Returns the indexes of the view’s currently visible items.

func cellForItem(at: Int) -> IKImageBrowserCell!

Returns the browser cell for the item at the specified index.

### Reordering and Groups Items

func selectionIndexes() -> IndexSet!

Returns the indexes of the selected cells.

func setSelectionIndexes(IndexSet!, byExtendingSelection: Bool)

Selects cells at the specified indexes.

func setAllowsMultipleSelection(Bool)

Controls whether the user can select more than one cell at a time.

func allowsMultipleSelection() -> Bool

Returns whether multiple selections are allowed.

func setAllowsEmptySelection(Bool)

Controls whether an empty selection is allowed.

func allowsEmptySelection() -> Bool

Returns whether an empty selection is allowed.

func setAllowsReordering(Bool)

Controls whether the user can reorder items.

func allowsReordering() -> Bool

Returns whether the user can reorder items.

func setAnimates(Bool)

Controls whether the receiver animates reordering and changes of the data source.

func animates() -> Bool

Returns whether the receiver animates reordering and changes of the data source.

func expandGroup(at: Int)

Expands a group at the specified index.

func collapseGroup(at: Int)

Collapses a group at the specified index.

func isGroupExpanded(at: Int) -> Bool

Returns whether the group at the provided index is expanded.

### Supporting Drag and Drop

func setDraggingDestinationDelegate(Any!)

Sets the dragging destination delegate of the receiver.

func draggingDestinationDelegate() -> Any!

Returns the dragging destination delegate of the receiver.

func setDrop(Int, dropOperation: IKImageBrowserDropOperation)

Allows the class to retarget the drop action.

func indexAtLocationOfDroppedItem() -> Int

Returns the index of the cell where the drop operation occurred.

func setAllowsDroppingOnItems(Bool)

Specifies whether the user can drop on items.

func allowsDroppingOnItems() -> Bool

Returns whether the user can drop on items.

func dropOperation() -> IKImageBrowserDropOperation

Returns the current drop operation.

### Core Animation Layer Integration

func setForegroundLayer(CALayer!)

The Core Animation layer used as the foreground overlay.

func foregroundLayer() -> CALayer!

Returns the foreground Core Animation layer

func setBackgroundLayer(CALayer!)

The Core Animation layer used as the view’s background.

func backgroundLayer() -> CALayer!

Returns the foreground Core Animation layer

### QuickLook Support

func setCanControlQuickLookPanel(Bool)

Specifies whether the view can automatically take control of the QuickLook panel.

func canControlQuickLookPanel() -> Bool

Returns whether the view can automatically take control of the QuickLook panel.

### Getting Columns and Rows Information

func numberOfColumns() -> Int

Returns the current number of columns.

func numberOfRows() -> Int

Returns the current number of rows.

func rect(ofColumn: Int) -> NSRect

Returns the rectangle containing the specified column.

func columnIndexes(in: NSRect) -> IndexSet!

Returns the column indexes in the specified rectangle.

func rect(ofRow: Int) -> NSRect

Returns the rectangle containing the specified row.

func rowIndexes(in: NSRect) -> IndexSet!

Returns the row indexes in the specified rectangle.

### Constants

Cell Appearance Style Masks

Masks for the appearance style bit field.

Group Style Attributes

Attributes for the group style. Used by the

View Options Keys

Keys for image browser view options. You set and retrieve values for these keys by sending the view `setValue:forKey` and `valueForKey:` messages.

Group Keys

Keys for group attributes.

struct IKImageBrowserDropOperation

These constants specify the locations for dropping items onto the browser view. Used by the method setDrop(_:dropOperation:).

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSDraggingSource
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

