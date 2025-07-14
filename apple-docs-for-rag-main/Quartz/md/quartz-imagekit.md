

- Quartz
-  ImageKit 

API Collection

# ImageKit

## Topics

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

class IKSlideshow

The `IKSlideshow` class encapsulates a data source and options for a slideshow.

### Protocols

protocol IKCameraDeviceViewDelegate

The `IKCameraDeviceViewDelegate` protocol is adopted by the delegate of the IKCameraDeviceView class. It allows downloading of camera content, handling selection changes, and handling errors.

protocol IKDeviceBrowserViewDelegate

The `IKDeviceBrowserViewDelegate` defines the methods that the delegate of the IKDeviceBrowserView class can implement. All the methods are optional.

protocol IKFilterCustomUIProvider

A protocol used to provide a custom UI.

IKImageBrowserDataSource Protocol

The `IKImageBrowserDataSource` informal protocol declares the methods that an instance of the IKImageBrowserView class uses to access the contents of its data source object.

IKImageBrowserDelegate Protocol

The `IKImageBrowserDelegate` is an informal protocol for the delegate of an IKImageBrowserView object. You can implement these methods to perform custom tasks when in response to events in the image browser view.

IKImageBrowserItem Protocol

The `IKImageBrowserItem` informal protocol declares the methods that an instance of the IKImageBrowserView class uses to access the contents of its data source for a given item. Some of the methods in this protocol are needed frequently, so you should implement them efficiently.

protocol IKImageEditPanelDataSource

The `IKImageEditPanelDataSource` protocol describes the methods that an IKImageEditPanel object uses to access the contents of its data source object.

protocol IKScannerDeviceViewDelegate

The `IKScannerDeviceViewDelegate` protocol defines the delegate protocol that the IKScannerDeviceView delegate must conform to.

protocol IKSlideshowDataSource

The `IKSlideshowDataSource` protocol describes the methods that an IKSlideshow object uses to access the contents of its data source object.

### Informal Protocols

struct IKImageBrowserCellState

The possible states for the browser cell. These values are used by the cellState() method.

struct IKImageBrowserDropOperation

These constants specify the locations for dropping items onto the browser view. Used by the method setDrop(_:dropOperation:).

### Extended Types

class CIFilter

An image processor that produces an image by manipulating one or more input images or by generating new image data.

### Reference

ImageKit Constants

Quartz Enumerations

### Deprecated symbols

class IKImageBrowserView

A view for displaying and browsing a large collection of images and movies.

Deprecated

