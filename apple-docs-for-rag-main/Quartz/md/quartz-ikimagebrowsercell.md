

- Quartz
-  IKImageBrowserCell 

Class

# IKImageBrowserCell

A class used to display a cell.

macOS 10.4+

``` source
class IKImageBrowserCell
```

## Overview

`A` class that is used to display a cell conforming to the IKImageBrowserItem Protocol in an IKImageBrowserView.

## Topics

### Cell Component Frames

func frame() -> NSRect

Returns the receiver’s frame rectangle, which defines its position in its IKImageBrowserView.

func imageFrame() -> NSRect

Returns the receiver’s image frame rectangle, which defines the position of the thumbnail in its IKImageBrowserView.

func subtitleFrame() -> NSRect

Returns the receiver’s subtitle frame rectangle.

func titleFrame() -> NSRect

Returns the receiver’s title frame rectangle.

func imageContainerFrame() -> NSRect

Returns the receiver’s image container frame rectangle, which defines the position of the container of the thumbnail.

### Represented Item

func indexOfRepresentedItem() -> Int

Returns the index of the receiver’s represented object in the datasource.

func representedItem() -> Any!

Returns the receiver’s represented object.

### Selection Handling

func isSelected() -> Bool

Returns whether the cell is selected.

func selectionFrame() -> NSRect

Returns the receiver’s selection frame rectangle, which defines the position of the selection rectangle in its IKImageBrowserView.

### Cell Content Display

func imageAlignment() -> NSImageAlignment

Returns the position of the cell’s image in the frame.

func opacity() -> CGFloat

Returns the opacity of the receiver.

### Getting The Cell State

func cellState() -> IKImageBrowserCellState

Returns the current cell state of the receiver.

### Core Animation Integration

func layer(forType: String!) -> CALayer!

Returns a layer for the specified position.

### Getting The Parent Browser View

func imageBrowserView() -> IKImageBrowserView!

Returns the view the receiver uses to display the cell.

### Constants

struct IKImageBrowserCellState

The possible states for the browser cell. These values are used by the cellState() method.

Cell Layer Positions

Optional positioning of additional layers displayed with the cell. Used by the layer(forType:) method.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Classes

class IKCameraDeviceView

The `IKCameraDeviceView` class displays the contents of the selected camera.

class IKDeviceBrowserView

The `IKDeviceBrowserView` allows you to select a camera or scanner from a list of the available devices.

class IKFilterBrowserPanel

Presents a user interface for browsing filters.

class IKFilterBrowserView

The `IKFilterBrowserView` class is used as a container for the elements of an IKFilterBrowserPanel object.

class IKFilterUIView

Input parameters for filtering core image filters.

class IKImageEditPanel

The `IKImageEditPanel` class provides a panel, that is, a utility window that floats on top of document windows, optimized for image editing.

class IKImageView

A view that allows displaying and minor editing of an image.

class IKPictureTaker

The `IKPictureTaker` class represents a panel that allows users to choose images by browsing the file system. The picture taker panel provides an Open Recent menu, supports image cropping, and supports taking snapshots from an iSight or other digital camera.

class IKSaveOptions

The `IKSaveOptions` class initializes, adds, and manages user interface options for saving image data.

class IKScannerDeviceView

The `IKScannerDeviceView` class displays a view that allows scanning. It can be customized by specifying the display mode. The delegate receives the scanned data and must implement the IKScannerDeviceViewDelegate protocol.

class IKSlideshow

The `IKSlideshow` class encapsulates a data source and options for a slideshow.

