

- Quartz
-  IKDeviceBrowserView 

Class

# IKDeviceBrowserView

The `IKDeviceBrowserView` allows you to select a camera or scanner from a list of the available devices.

macOS 10.6+

``` source
@MainActor
class IKDeviceBrowserView
```

## Overview

The IKDeviceBrowserView delegate must conform to the IKDeviceBrowserViewDelegate protocol. The delegate provides methods to inform you of selection changes in the browser as well as errors encountered when creating the browser list.

## Topics

### Getting the Selected Device

var selectedDevice: ICDevice!

Returns the selected device.

### Specifying the Device Types to Display

var displaysLocalCameras: Bool

Specifies whether local cameras are displayed by the browser.

var displaysNetworkCameras: Bool

Specifies whether network cameras are displayed by the browser.

var displaysLocalScanners: Bool

Specifies whether local scanners are displayed by the browser.

var displaysNetworkScanners: Bool

Specifies whether network scanners are displayed by the browser.

### Specifying the Display Mode

var mode: IKDeviceBrowserViewDisplayMode

Specifies the browser display mode.

### Getting and Setting the Delegate

var delegate: (any IKDeviceBrowserViewDelegate)!

Specifies the delegate object.

### Constants

enum IKDeviceBrowserViewDisplayMode

These constants specify the display mode of the device browser.

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

class IKFilterBrowserPanel

Presents a user interface for browsing filters.

class IKFilterBrowserView

The `IKFilterBrowserView` class is used as a container for the elements of an IKFilterBrowserPanel object.

class IKFilterUIView

Input parameters for filtering core image filters.

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

