

- Quartz
-  IKScannerDeviceView 

Class

# IKScannerDeviceView

The `IKScannerDeviceView` class displays a view that allows scanning. It can be customized by specifying the display mode. The delegate receives the scanned data and must implement the IKScannerDeviceViewDelegate protocol.

macOS 10.6+

``` source
@MainActor
class IKScannerDeviceView
```

## Topics

### Setting the Scanner Device

var scannerDevice: ICScannerDevice!

The device used for scanning

### Setting the Device View’s Display Mode

var mode: IKScannerDeviceViewDisplayMode

The display mode used by the device view.

var hasDisplayModeAdvanced: Bool

The property that determines whether the scanner view uses the advanced display mode.

var hasDisplayModeSimple: Bool

The property that determines whether the scanner view uses the simple display mode.

### Configuring Downloading

var displaysDownloadsDirectoryControl: Bool

Determines whether the downloads directory control is displayed.

var downloadsDirectory: URL!

The directory where scans are saved.

var transferMode: IKScannerDeviceViewTransferMode

Determines how the scanned content is provided to the delegate.

var documentName: String!

Returns the document name.

### Specifying a Post Processing Application

var displaysPostProcessApplicationControl: Bool

Specifies whether the post processing application control is displayed.

var postProcessApplication: URL!

The URL of the application to use for post processing of the scan.

### Getting and Setting the Delegate

var delegate: (any IKScannerDeviceViewDelegate)!

The scanner device delegate

### Customizing Button Labels

var overviewControlLabel: String!

Allows customization of the “Overview” label.

var scanControlLabel: String!

Allows customization of the “Scan” label.

### Constants

enum IKScannerDeviceViewTransferMode

These constants determine how the scanner data is returned to the delegate. They are used by the transferMode property.

enum IKScannerDeviceViewDisplayMode

These constants specify the display mode the scanner view will use. They are used by the mode property.

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

class IKSlideshow

The `IKSlideshow` class encapsulates a data source and options for a slideshow.

