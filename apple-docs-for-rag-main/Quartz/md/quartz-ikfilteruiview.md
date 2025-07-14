

- Quartz
-  IKFilterUIView 

Class

# IKFilterUIView

Input parameters for filtering core image filters.

macOS 10.4+

``` source
@MainActor
class IKFilterUIView
```

## Overview

The `IKFilterUIView` class provides a view that contains input parameter controls for a Core Image filter (CIFilter). You need to use this class when providing a user interface for a custom filter. The class creates a view that has an object controller for the given filter. It also retains the filter.

## Topics

### Creating and Initializing a Filter UI View

class func view(withFrame: NSRect, filter: CIFilter!) -> Any!

Creates a view that contains controls for the input parameters of a filter.

init!(frame: NSRect, filter: CIFilter!)

Initializes a view that contains controls for the input parameters of a filter.

### Getting Data from the Filter View

func filter() -> CIFilter!

Returns the Core Image filter associated with the view.

func objectController() -> NSObjectController!

Returns the object controller for the bindings between the filter and its view.

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
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

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

class IKImageBrowserCell

A class used to display a cell.

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

