

- Quartz
-  IKSaveOptions 

Class

# IKSaveOptions

The `IKSaveOptions` class initializes, adds, and manages user interface options for saving image data.

macOS 10.5+

``` source
class IKSaveOptions
```

## Topics

### Creating A Save Options Accessory View

init!(imageProperties: [AnyHashable : Any]!, imageUTType: String!)

Initializes a save options accessory pane for the provided image properties and uniform type identifier.

func addAccessoryView(to: NSSavePanel!)

Adds `IKSaveOptions` accessory view to a `NSSavePanel`.

### Retrieving User Responses

var imageProperties: [AnyHashable : Any]!

Returns a dictionary of updated image properties that reflects the user’s selection.

var imageUTType: String!

Returns the uniform type identifier that reflects the user’s selection.

var userSelection: [AnyHashable : Any]!

Returns a dictionary that contains the save options selected by the user.

### Getting and Setting the delegate

var delegate: AnyObject!

Specifies the delegate object.

### File Type Filtering

func saveOptions(_ saveOptions: IKSaveOptions!, shouldShowUTType utType: String!) -> Bool

Called to determine if the specified uniform type identifier should be shown in the save panel.

### Instance Properties

var rememberLastSetting: Bool

### Instance Methods

func add(to: NSView!)

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

class IKImageBrowserCell

A class used to display a cell.

class IKImageEditPanel

The `IKImageEditPanel` class provides a panel, that is, a utility window that floats on top of document windows, optimized for image editing.

class IKImageView

A view that allows displaying and minor editing of an image.

class IKPictureTaker

The `IKPictureTaker` class represents a panel that allows users to choose images by browsing the file system. The picture taker panel provides an Open Recent menu, supports image cropping, and supports taking snapshots from an iSight or other digital camera.

class IKScannerDeviceView

The `IKScannerDeviceView` class displays a view that allows scanning. It can be customized by specifying the display mode. The delegate receives the scanned data and must implement the IKScannerDeviceViewDelegate protocol.

class IKSlideshow

The `IKSlideshow` class encapsulates a data source and options for a slideshow.

