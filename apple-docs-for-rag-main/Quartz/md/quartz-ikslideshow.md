

- Quartz
-  IKSlideshow 

Class

# IKSlideshow

The `IKSlideshow` class encapsulates a data source and options for a slideshow.

macOS 10.4+

``` source
class IKSlideshow
```

## Topics

### Creating a Shared Instance of a Slideshow

class func shared() -> IKSlideshow!

Returns a shared instance of a slideshow.

### Running and Stopping a Slideshow

func run(with: (any IKSlideshowDataSource)!, inMode: String!, options: [AnyHashable : Any]!)

Runs a slideshow that contains the specified kind of items, provided from a data source.

func stop(Any!)

Stops a slideshow.

var autoPlayDelay: TimeInterval

Controls the interval of time before a slideshow starts to play automatically.

### Getting Slideshow Data

func indexOfCurrentSlideshowItem() -> Int

Returns the index of the current slideshow item.

### Reloading Data

func reloadData()

Reloads the data for a slideshow.

func reloadItem(at: Int)

Reloads the data for a slideshow, starting at the specified index.

### Exporting Slideshow Items

class func canExport(toApplication: String!) -> Bool

Finds out whether the slideshow can export its contents to an application.

class func exportItem(Any!, toApplication: String!)

Exports a slideshow item to the application that has the provided bundle identifier.

### Constants

Bundle Identifiers

Identifiers for exporting slideshow items to an application.

Slideshow Modes

The kind of items in the slideshow.

Slideshow Option Keys

Keys for slideshow options.

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

class IKSaveOptions

The `IKSaveOptions` class initializes, adds, and manages user interface options for saving image data.

class IKScannerDeviceView

The `IKScannerDeviceView` class displays a view that allows scanning. It can be customized by specifying the display mode. The delegate receives the scanned data and must implement the IKScannerDeviceViewDelegate protocol.

