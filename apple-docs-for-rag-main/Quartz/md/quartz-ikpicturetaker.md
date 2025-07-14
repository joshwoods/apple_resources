

- Quartz
-  IKPictureTaker 

Class

# IKPictureTaker

The `IKPictureTaker` class represents a panel that allows users to choose images by browsing the file system. The picture taker panel provides an Open Recent menu, supports image cropping, and supports taking snapshots from an iSight or other digital camera.

macOS 10.4+

``` source
@MainActor
class IKPictureTaker
```

## Topics

### Creating And Displaying The Picture Taker

class func pictureTaker() -> IKPictureTaker!

Returns a shared `IKPictureTaker` instance, creating it if necessary.

func beginSheet(for: NSWindow!, withDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Opens a picture taker as a sheet whose parent is the specified window.

func begin(withDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Opens a picture taker pane.

func popUpRecentsMenu(for: NSView!, withDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Displays the Open Recent popup menu associated with the picture taker.

func runModal() -> Int

Opens a modal picture taker dialog.

### Getting and Setting Images

func setInputImage(NSImage!)

Set the image input for the picture taker.

func inputImage() -> NSImage!

Returns the input image associated with the picture taker.

func outputImage() -> NSImage!

Returns the edited image.

### Getting and Setting Mirroring

func setMirroring(Bool)

Controls whether the receiver enables video mirroring during snapshots.

func mirroring() -> Bool

Returns whether video mirroring is enabled during snapshots.

### Constants

Picture Taker Keys

Keys for customizing the picture taker appearance and behavior. These values are set by sending the picture taker instance `setValue:forKey`.

## Relationships

### Inherits From

- NSPanel

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
- NSMenuItemValidation
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- NSUserInterfaceValidations
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

class IKSaveOptions

The `IKSaveOptions` class initializes, adds, and manages user interface options for saving image data.

class IKScannerDeviceView

The `IKScannerDeviceView` class displays a view that allows scanning. It can be customized by specifying the display mode. The delegate receives the scanned data and must implement the IKScannerDeviceViewDelegate protocol.

class IKSlideshow

The `IKSlideshow` class encapsulates a data source and options for a slideshow.

