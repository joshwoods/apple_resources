

- Quartz
-  IKCameraDeviceView 

Class

# IKCameraDeviceView

The `IKCameraDeviceView` class displays the contents of the selected camera.

macOS 10.6+

``` source
@MainActor
class IKCameraDeviceView
```

## Topics

### Getting and Setting the Camera Device

var cameraDevice: ICCameraDevice!

The current camera device.

### View Display Mode

var iconSize: Int

Specifies the icon size.

var mode: IKCameraDeviceViewDisplayMode

Specifies the display mode of the camera device view.

var hasDisplayModeIcon: Bool

Returns whether the device view is being displayed in icon mode.

var hasDisplayModeTable: Bool

Returns whether the device view is being displayed in table mode.

### Selecting the File Transfer Mode

var transferMode: IKCameraDeviceViewTransferMode

Determines how the contents are saved by the delegate.

### Configuring Download Interface and Downloading Files

var canDownloadSelectedItems: Bool

Returns whether the selected items can be downloaded

var downloadsDirectory: URL!

Specifies the directory where files are downloaded

func downloadSelectedItems(Any!)

Deletes the selected items from the camera.

func downloadAllItems(Any!)

Downloads all the items.

var downloadSelectedControlLabel: String!

Allows the “Download Selected” control to be renamed.

var downloadAllControlLabel: String!

Allows the “Download All” control to be renamed.

var displaysDownloadsDirectoryControl: Bool

Specifies whether the downloads directory control should be displayed.

### Getting and Setting the Post Processing Application

var displaysPostProcessApplicationControl: Bool

Displays whether the post process application control should be displayed.

var postProcessApplication: URL!

The URL of the application used to post process the image.

### Deleting Selected Items

var canDeleteSelectedItems: Bool

Returns whether the selected items can be deleted.

func deleteSelectedItems(Any!)

Deletes the currently selected items.

### Selection Management

func select(IndexSet!, byExtendingSelection: Bool)

Invoked to select the specified files, extending the selection if specified.

func selectedIndexes() -> IndexSet!

The selected indexes of the camera files.

### Getting and Setting the Delegate

var delegate: (any IKCameraDeviceViewDelegate)!

The camera device view delegate.

### Selected Item Rotation

var canRotateSelectedItemsLeft: Bool

Returns whether the selected items can be rotated left.

var canRotateSelectedItemsRight: Bool

Returns whether the selected items can be rotated right.

func rotateLeft(Any!)

Rotates the selected image to the left.

func rotateRight(Any!)

Rotates the selected image to the right.

### Constants

enum IKCameraDeviceViewDisplayMode

These constants specify the display mode used by the camera view. These constants are used by mode.

enum IKCameraDeviceViewTransferMode

These constants specify the transfer mode used by the camera view. These constants are used by mode.

### Instance Methods

func setCustomActionControl(NSSegmentedControl!)

func setCustomDelete(NSSegmentedControl!)

func setCustomIconSizeSlider(NSSlider!)

func setCustomModeControl(NSSegmentedControl!)

func setCustomRotateControl(NSSegmentedControl!)

func setShowStatusInfoAsWindowSubtitle(Bool)

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

## See Also

### Classes

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

class IKScannerDeviceView

The `IKScannerDeviceView` class displays a view that allows scanning. It can be customized by specifying the display mode. The delegate receives the scanned data and must implement the IKScannerDeviceViewDelegate protocol.

class IKSlideshow

The `IKSlideshow` class encapsulates a data source and options for a slideshow.

