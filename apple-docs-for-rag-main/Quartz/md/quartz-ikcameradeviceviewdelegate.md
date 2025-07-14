

- Quartz
-  IKCameraDeviceViewDelegate 

Protocol

# IKCameraDeviceViewDelegate

The `IKCameraDeviceViewDelegate` protocol is adopted by the delegate of the IKCameraDeviceView class. It allows downloading of camera content, handling selection changes, and handling errors.

macOS 10.4+

``` source
protocol IKCameraDeviceViewDelegate
```

## Topics

### Downloading Camera Content

func cameraDeviceView(IKCameraDeviceView!, didDownloadFile: ICCameraFile!, location: URL!, fileData: Data!, error: (any Error)!)

Invoked for each file that is downloaded from the camera device.

### Detecting Selection Changes

func cameraDeviceViewSelectionDidChange(IKCameraDeviceView!)

Invoked when the selection changed.

### Managing Errors

func cameraDeviceView(IKCameraDeviceView!, didEncounterError: (any Error)!)

Invoked when the camera encounters an error.

## See Also

### Protocols

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

