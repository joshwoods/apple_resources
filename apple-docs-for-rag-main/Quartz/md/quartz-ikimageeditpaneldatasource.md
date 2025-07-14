

- Quartz
-  IKImageEditPanelDataSource 

Protocol

# IKImageEditPanelDataSource

The `IKImageEditPanelDataSource` protocol describes the methods that an IKImageEditPanel object uses to access the contents of its data source object.

macOS 10.4+

``` source
protocol IKImageEditPanelDataSource
```

## Topics

### Getting and Setting Image Properties

var imageProperties: [AnyHashable : Any]!

Returns a dictionary of the image properties associated with the image in the image edit panel.

func setImage(CGImage!, imageProperties: [AnyHashable : Any]!)

Sets an image with the specified properties.

**Required**

### Getting Images From the Data Source

var image: CGImage!

Returns an image.

**Required**

func thumbnail(withMaximumSize: NSSize) -> Unmanaged&lt;CGImage>!

Returns a thumbnail image whose size is no larger than the specified size.

### New Methods

var hasAdjustMode: Bool

Returns whether the adjust mode view tab should be displayed.

var hasDetailsMode: Bool

Returns whether the details mode view tab should be displayed.

var hasEffectsMode: Bool

Returns whether the effects mode view tab should be displayed.

## See Also

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

protocol IKScannerDeviceViewDelegate

The `IKScannerDeviceViewDelegate` protocol defines the delegate protocol that the IKScannerDeviceView delegate must conform to.

protocol IKSlideshowDataSource

The `IKSlideshowDataSource` protocol describes the methods that an IKSlideshow object uses to access the contents of its data source object.

